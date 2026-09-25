# CDC Disease Sentinel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cdc-disease-sentinel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Detect disease surges in US public health data. CDC's weekly NNDSS case counts with trend, 52-week baseline, YTD comparison and a surge multiplier per disease, state or region — keyless, stateless.

## Description
CDC Disease Sentinel watches the CDC's National Notifiable Diseases Surveillance System so your agent can answer the question people keep asking: is anything spiking right now, and where?

### What you can do

- **See what's surging** — one call gives the latest week's case count, its average over a lookback window, and the multiplier: surge, elevated, or normal
- **Compare against the year** — the dataset's own 52-week maximum and YTD vs the same period last year, with a plain-language verdict
- **Zoom into one state** — national, any state, or a census region, with the exact area names returned so follow-ups never guess
- **Read the curve** — the last N weeks of a disease as a compact series, so you see momentum, not just the latest number

### How it works

1. Subscribe to this server (no credential, no account — the dataset is public CDC open data)
2. Ask "is anything spiking this week?" — the surge check runs against the configured disease(s)
3. Re-run any time; the server computes everything from the live weekly series and keeps no state

### Who is this for?

- **Public-health watchers** — journalists, analysts, and the just-anxious curious who want to know what's actually moving, not headlines
- **Agents & automations** — a scheduled "disease pulse" digest with deltas computed server-side
- **Researchers** — reproducible weekly series with the source's own flags and caveats preserved


## Available Tools (5)
- **list_diseases**: The labels here are the exact strings the other tools expect — copy one into disease_trend, disease_baseline, surge_check or state_scan instead of inventing a name. MMWR years run July-to-June; use year to look at the previous MMWR year.

The NNDSS diseases currently tracked by CDC weekly surveillance, with this week's national case counts
- **disease_baseline**: Use this for the "is this unusual?" question — the ratio of YTD to the same period last year is the clearest signal.

Where a disease stands right now: latest week vs the 52-week maximum and YTD vs the same period last year
- **disease_trend**: Use this to see the shape of the curve: is the count climbing, flat, or collapsing? Weeks without a reported case show "no data" rather than a fabricated zero.

Weekly case counts for one disease over the last N MMWR weeks, national or one state
- **state_scan**: Areas with no reported cases show 0. The area names returned here are the exact strings to use as the state parameter of the other tools. Use this for "where is it concentrated?" questions, and to discover the exact area spelling for a follow-up.

Where a disease is most reported in one week: every reporting area ranked by case count
- **surge_check**: Verdicts: "surge" at or above threshold (default 2.0x), "elevated" at half the threshold, "normal" below that, plus special cases (no cases this week, or new cases where the baseline had none). This is the tool for "is X spiking right now?" — set threshold lower for early-warning sensitivity (e.g. 1.5) or higher to only flag true surges (3-5).

Surge detector: latest week's count vs the average of the prior N weeks, with a multiplier verdict


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CDC Disease Sentinel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there a disease surge this week anywhere in the US?"

**🤖 AI Agent:**
> Runs surge_check on the configured disease (or walks a few from list_diseases) and reports the multiplier verdicts.

---

**👤 You:**
> "Show me the last 16 weeks of national meningitis cases and say if it's trending up."

**🤖 AI Agent:**
> Uses disease_trend with weeks=16 and interprets the series shape.

---

**👤 You:**
> "Which states report the most norovirus this week?"

**🤖 AI Agent:**
> Uses state_scan for norovirus and lists the ranked areas with case counts.


## ❓ FAQ

**Q: Do I need credentials?**
No. The dataset is public CDC open data on Socrata, readable without a token (anonymous access is throttled and capped at 500 rows per query — every tool stays well under that). No signup, no key, no per-user state.

**Q: How does the surge detector decide "surge"?**
It divides the latest week's reported cases by the average of the previous N weeks (default 12, configurable). At or above the threshold multiplier (default 2.0) it reports a surge; at half the threshold it reports elevated; special cases (no cases this week, or a baseline with zero cases) are called out explicitly instead of producing a division artifact.

**Q: Why do the tools insist on "exact" disease and area names?**
The CDC portal's query engine only matches values exactly (fuzzy matching silently returns nothing), so list_diseases returns the exact labels to copy, and state_scan returns the exact area names — follow-up calls just copy one of them instead of guessing. If a name doesn't match you get an error that says so, never an empty silent answer.

**Q: What data is behind it?**
CDC's NNDSS weekly surveillance: reported notifiable-disease case counts per MMWR week, per geography (national, regions, states, New York City), plus the dataset's own 52-week maximum and YTD comparators. Weeks without reported cases are shown as "no data", not as zeros. MMWR years run July-to-June.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cdc-disease-sentinel](https://vinkius.com/en/ai-agent-connect/cdc-disease-sentinel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CDC Disease Sentinel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cdc-disease-sentinel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CDC Disease Sentinel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cdc-disease-sentinel": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
