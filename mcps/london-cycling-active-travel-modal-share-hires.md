# London Cycling & Active Travel: Modal Share & Hires MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/london-cycling-active-travel-modal-share-hires)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless London active-travel data: walking and cycling trip shares by local authority on the 2010/11 and 2017/18 surveys, plus TFL's daily bicycle-hire series (Sycamore) with per-year totals and the busiest day.

## Description
Two official London active-travel datasets — keyless, straight from the London open-data platform (data.london.gov.uk).

### What you can do
- **active_travel_rates / active_travel_lookup / active_travel_ranking** — the walking and cycling shares of trips by local authority on the 2010/11 and 2017/18 Active Travel surveys, at the 5x-, 20x- and 40x-per-week frequencies: the full paged series, one authority's history, and the ranking of authorities on one year (city-wide aggregate rows excluded)
- **bicycle_hires_daily / bicycle_hires_by_year** — TFL's daily bicycle-hire counts: the day series bounded by ISO dates, and per-year totals with the busiest day of each year
- **active_travel_overview** — both datasets in one call: the 2017/18 5x-per-week authority averages plus the hire totals, first/last hire day and the busiest day overall

### Who is this for
Mobility planners, urban journalists and researchers comparing a borough's active-travel uptake over time or benchmarking hire demand by year. Years are stored as Excel serials in the source files and mapped to financial-year labels (2010/11, 2017/18) by the tools; the hire dates are real calendar days, so filter with ordinary ISO dates.


## Available Tools (6)
- **active_travel_lookup**: la is required, matched case-insensitively.

Walking/cycling time series for one local authority
- **active_travel_overview**: Use the dedicated tools to drill down.

Headline numbers across the London cycling datasets
- **active_travel_ranking**: Aggregate areas (London, Inner/Outer London, England) are excluded. Returns the top and bottom N areas.

Rank local authorities by cycling rate
- **active_travel_rates**: 5x per week). Areas include the 33 London boroughs plus aggregates. Optional la (exact, case-insensitive), year ("2017/18") and frequency. Page with limit/offset.

GLA walking and cycling rates per local authority
- **bicycle_hires_by_year**: Years 2010 (partial) to the latest published year.

Annual Santander Cycles hire totals
- **bicycle_hires_daily**: Optional ISO date bounds (from, to, "YYYY-MM-DD"). Page with limit/offset (1,000 days max per call).

Daily Santander Cycles (formerly Cycle Hire) totals in London


## 💬 Prompt Examples

Here are some examples of how you can interact with the **London Cycling & Active Travel: Modal Share & Hires** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What share of Newham trips are by bicycle in 2017/18?"

**🤖 AI Agent:**
> Call active_travel_lookup with la "Newham" — the series across the survey years comes back with the walking and cycling shares at each frequency; read the 2017/18 row at 5x per week.

---

**👤 You:**
> "Which day had the most bicycle hires?"

**🤖 AI Agent:**
> Run bicycle_hires_by_year — every year block carries its total and its busiest day; the latest block's busiest day is the answer for the most recent year.

---

**👤 You:**
> "Compare cycling uptake across London boroughs."

**🤖 AI Agent:**
> Call active_travel_ranking — the top side lists the boroughs with the highest cycling share and the bottom side the lowest, both at the 2017/18 5x-per-week slice by default.


## ❓ FAQ

**Q: Do I need an API key?**
No. data.london.gov.uk publishes every dataset as an anonymous file download (CSV or Excel). This MCP defines no credentials and needs nothing configured.

**Q: What do the 5x / 20x / 40x per week frequencies mean?**
The survey asks respondents how many times per week they walk or cycle. 5x-per-week is the everyday-use slice and the default for the ranking and overview tools; 20x and 40x are the heavier-use slices. Pick the frequency you are comparing.

**Q: Which hire scheme is in the daily series?**
The TFL daily counts come from the city's Sycamore (dockless) hire scheme: each row is one calendar day and the hires recorded that day. Per-year totals and the busiest day come from aggregating those rows.

**Q: Why are London, Inner London and England out of the ranking?**
The ranking compares local authorities against each other; the city-wide and England rows are aggregates, not an authority, so they are excluded by default. Use active_travel_lookup to read those aggregate rows directly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/london-cycling-active-travel-modal-share-hires](https://vinkius.com/en/ai-agent-connect/london-cycling-active-travel-modal-share-hires)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **London Cycling & Active Travel: Modal Share & Hires** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `london-cycling-active-travel-modal-share-hires` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **London Cycling & Active Travel: Modal Share & Hires** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "london-cycling-active-travel-modal-share-hires": {
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
