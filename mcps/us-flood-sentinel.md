# US Flood Sentinel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/us-flood-sentinel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Know when US rivers are actually flooding: USGS gage heights checked against their flood stages, multi-day trends, and every active NWS flood alert nationwide — with since-based deltas so the agent re-checks and reports only what changed. Keyless, stateless.

## Description
US Flood Sentinel answers the question nobody wants to learn the hard way: is my river (or a flood warning) actually moving right now? It joins two public US sources — USGS Water Data and the National Weather Service — into one stateless sentinel your agent can re-check on a schedule.

### What you can do

- **Find the river you care about** — stream gages in any US state, biggest drainage area first, name-filtered to a river or town (the gages that flood are the big ones)
- **Now-status of one gage** — latest gage height against the flood stage on file, with a verdict: normal, within 1 ft of stage, or above flood stage
- **Multi-day trend** — daily min/max/mean for the last N days, an overall direction verdict, and how many days the river ran over flood stage
- **Nationwide flood alerts** — every active NWS flood alert (FloodWarning, FloodWatch, excess and coastal variants), or one event type only
- **What changed since I asked** — pass the timestamp of your last check and get the alerts issued since then, split into still-active vs since-expired

### How it works

1. Subscribe (no credential, no account — both APIs are public)
2. Ask "is anything flooding?" — one call returns the active alerts nationwide
3. For your river: find the gage, check its now-status and trend; keep the timestamp in context and re-run with `since` to get only the delta

### Who is this for?

- **People near rivers and coasts** — property owners, campers, boaters who want the water-level number, not just a news headline
- **Agents & automations** — a scheduled flood pulse: alerts + your gage list, deltas only, no full re-reads
- **Emergency managers & planners** — the all-events alert sweep and exceedance-day counts as machine-readable inputs


## Available Tools (6)
- **current_gage**: It also reports the thresholds on file. The USGS continuous feed is sparse, so a quiet gage answers with status no_data or stale_data and a note instead of a number — that is a finding, not an error. Pass the gage id from find_gages (USGS-########) or just the site number.

Now-status of one USGS gage: latest gage height against its flood stage, with a verdict
- **gage_trend**: The USGS daily summaries are sparse per gage: when a gage does not publish them the tool falls back to its continuous observations and says so in the note. Use it to answer "is the river still rising?" after current_gage shows a high reading.

Multi-day gage-height trend for one USGS gage, with direction and flood-stage exceedance days
- **find_gages**: Pass the state as a name ("California") or FIPS code (06); narrow with a river or place-name fragment. Each row carries the gage id that current_gage and gage_trend take as their gage parameter, plus the site number, name, county and drainage area.

Find USGS stream gages in a US state, biggest drainage area first, optionally name-filtered
- **flood_alerts**: Pass event to watch one type only. Zero results is a meaningful answer: no flood alert is active in the US right now. The agent should re-run this (or use flood_delta) at its next check to catch new issues.

All active NWS flood alerts across the US, optionally one event type only
- **flood_delta**: The NWS recent-alerts feed keeps only the newest alerts, so a baseline older than the feed window may miss some — the result says so.

NWS flood alerts issued or updated since your last check, split into still-active vs since-expired
- **flood_watch**: — the full list is returned) and it answers whether any of that type is active in the US right now, with the full alert details when there are some. A quiet result is "No <event> is active in the US right now." Scheduled watches run this one call per event type.

Watch one NWS flood event type across the US: verdict plus the active alerts of that type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Flood Sentinel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is anything flooding in the US right now?"

**🤖 AI Agent:**
> Runs flood_alerts (all flood event types) and reports the active alerts with their areas, or confirms there are none.

---

**👤 You:**
> "How close to flood stage is the Colorado River near Yuma?"

**🤖 AI Agent:**
> Runs find_gages (California/Arizona, "colorado") then current_gage on the matching gage and reports the margin to flood stage.

---

**👤 You:**
> "My gage was 18 ft yesterday 06:00 UTC — what has happened since?"

**🤖 AI Agent:**
> Runs gage_trend with a window covering the baseline and, for the river, flood_delta from that timestamp.


## ❓ FAQ

**Q: Do I need credentials?**
No. Both the USGS Water Data OGC API and the NWS alerts API are public with no key, no account. Anonymous NWS access is rate-limited to roughly 30 requests per minute, so the all-events sweep is kept to a handful of calls.

**Q: How does the "since" delta detection work?**
The server is stateless. Any tool that returns an as_of or sent timestamp is your baseline: keep it in the agent's context, and on the next check pass it as since. flood_delta then returns only the alerts issued after that moment, split into still-active and since-expired — the agent reports the change, not the whole picture again.

**Q: Which rivers and gages are covered?**
Every US stream gage that publishes public USGS data — find_gages lists them per state, biggest drainage area first, so the rivers that actually flood (Colorado, Sacramento, Columbia, Missouri, ...) come on top. One honest caveat: USGS daily summaries and continuous feeds are sparse per gage; a gage without recent data answers "no data" with a note instead of failing.

**Q: Why are flood alerts nationwide instead of by state?**
The NWS API's 2026 revision dropped the state query parameter, so alert sweeps run by event type across the whole country. State-level precision lives in the USGS side of the sentinel: find_gages filters gages by state (and drainage area), so "is my county's river rising?" is answered by the gage, while "is anything flooding in the US?" is answered by the alerts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/us-flood-sentinel](https://vinkius.com/en/ai-agent-connect/us-flood-sentinel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Flood Sentinel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-flood-sentinel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Flood Sentinel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-flood-sentinel": {
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
