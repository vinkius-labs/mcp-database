# BPstat Banco de Portugal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bpstat-banco-de-portugal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Banco de Portugal's official statistics API: interest rates, inflation metrics, monetary aggregates, balance of payments, credit, reserves and national financial accounts — navigable by domain tree, with time-series observations, zero-auth.

## Description
**BPstat** is the statistical database of **Banco de Portugal** — the country's central bank and the authoritative source for Portuguese monetary and financial statistics.

### What you can do
- **Navigate the domain tree** — 77 statistical domains: national financial accounts, external statistics, balance of payments, payment systems, cash issuance, international reserves and more
- **Discover series** — list the statistical series in each domain (paginated), with last observation value and dimensional breakdowns (sector, instrument, country, maturity...)
- **Inspect metadata** — full series metadata: description, source, min/max observations, latest value and dimensional member combination
- **Pull time series** — observations as CSV with date-range filters (start_date/end_date), one or multiple series per call
- **Get the latest figure** — a lightweight latest-value tool that returns just the most recent reference date and value per series

### Why BPstat?
For Portuguese interest rates (including the famous Lisbor), monetary aggregates, bank credit to the economy, balance of payments, external reserves and financial accounts, Banco de Portugal is the primary source — the same data used by economists, journalists and the ECB. All of it without authentication.

### Who is this for?
Economists, financial analysts, journalists covering the Portuguese economy, fintechs, researchers, and AI agents that need authoritative Portuguese/central-bank statistics rather than second-hand aggregators.


## Available Tools (5)
- **list_statistical_domains**: Root domains have parent_id null; use parent_id to see sub-domains. Use a domain id in list_domain_series.

List BPstat statistical domains (monetary, external, interest rates, payments, reserves...)
- **list_domain_series**: Use links.next/previous (returned in data) to navigate pages — never fetch all pages. Get domain ids from list_statistical_domains.

List statistical series within a BPstat domain (paginated)
- **get_series_metadata**: g. sector, instrument, country). Comma-separate up to 10 series ids.

Get full metadata of BPstat statistical series (source, breakdown, last value)
- **get_series_observations**: Filter with start_date/end_date (YYYY-MM-DD) to control payload size. Comma-separate series ids.

Get time-series observations (values over time) from BPstat, as CSV
- **get_latest_values**: Use this instead of get_series_observations when you just need the current figure (e.g. latest interest rate, latest inflation).

Get the latest value of each BPstat series (lightweight JSON)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BPstat Banco de Portugal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the latest value of BPstat series 12456320 and what does it measure?"

**🤖 AI Agent:**
> 🏦 **Series 12456320 (BPstat)**

**What it measures:** Net lending/net borrowing of the total economy — accumulated transactions (national financial accounts domain).

**Latest value:** 2.38 (2026-03-31)
**Range:** min -12.5 (2012 crisis peak) → max 6.9

A positive value means the Portuguese economy as a whole is a net lender — a strong recovery signal compared to the sovereign-debt crisis years.

---

**👤 You:**
> "Pull the 2025 monthly history of debt securities stock series 12834303"

**🤖 AI Agent:**
> 📈 **Series 12834303 — Stock of debt securities, 2025 (BPstat)**

Unit: millions of euros

Jan 523.94 · Feb 527.93 · Mar 527.05 · ... · Dec 538.12

Trend: +2.7% over the year, steady monthly growth. I can compare with a benchmark series or break it down by issuer if you want.

---

**👤 You:**
> "What statistical domains does Banco de Portugal publish and where are interest rates?"

**🤖 AI Agent:**
> 🏦 **BPstat domain tree (77 domains)**

Root domains: National financial accounts · External statistics (→ Balance of payments, IIP, International reserves) · Payment systems and instruments · Cash issuance · International banking statistics...

**Interest rates** live in their own domain — I listed its series and found Lisbor and retail bank rate series. Want the latest Lisbor value?


## ❓ FAQ

**Q: Do I need an API key or registration?**
No. BPstat's data API is fully public — every tool in this MCP works without authentication or account.

**Q: How do I find the series id I need?**
Start with list_statistical_domains, then list_domain_series for the domain you care about. Each series entry includes its id, title and last value. You can also browse bpstat.bportugal.pt/pt/dados/explorer in a browser and copy the series id from the URL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bpstat-banco-de-portugal](https://vinkius.com/ai-agent-connect/bpstat-banco-de-portugal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BPstat Banco de Portugal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bpstat-banco-de-portugal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BPstat Banco de Portugal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bpstat-banco-de-portugal": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
