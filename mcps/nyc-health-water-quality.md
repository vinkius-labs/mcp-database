# NYC Health & Water Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-health-water-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC health data: seasonal flu vaccination sites, leading causes of death, drinking water quality samples, Cryptosporidium & Giardia monitoring, annual water consumption and DOHMH community health centers — no API key.

## Description
New York City public-health and water records, keyless.

### What you can do
- **Flu vaccination sites** — seasonal locations offering flu shots, with walk-in, insurance and children flags, address and phone
- **Leading causes of death** — by year, sex and race/ethnicity, with deaths, death rate and age-adjusted rate (years 2007–2021)
- **Drinking water quality** — distribution monitoring samples: residual chlorine, turbidity, coliform and E. coli counts, by site and class
- **Cryptosporidium & Giardia** — DEP water-quality monitoring results by site and date
- **Water consumption** — the annual trend: city population, total consumption in million gallons per day and per-capita gallons
- **Community health centers** — DOHMH centers with hours, walk-in acceptance, languages and website

### Who is this for
Public-health research, water-quality monitoring analysis and health-service planning. Water datasets are long-running, so sample searches apply a 365-day window by default; causes-of-death statistics are historical (2007–2021).


## Available Tools (6)
- **get_water_consumption_trends**: A small trend table; optionally pin one year. Use it to compare water use across years or build a per-capita trend.

NYC annual water consumption trends
- **list_flu_vaccination_sites**: The list is seasonal and refreshed each flu season — filter by borough, walk-in, insurance or children.

List NYC locations providing seasonal flu vaccinations
- **list_health_centers**: g. "Walk-ins accepted. Appointments preferred."), languages offered and website. Filter by borough or walk-in acceptance (partial match, e.g. "walk-in").

List NYC DOHMH community health centers
- **search_cryptosporidium_giardia**: The dataset is long, so a sample-date window is applied by default (365 days back).

Search NYC Cryptosporidium and Giardia monitoring results
- **search_drinking_water_quality**: coli counts. The dataset is long, so a sample-date window is applied by default (365 days back); narrow with sample site or class.

Search NYC drinking water quality distribution samples
- **search_leading_causes_of_death**: Years run 2007-2021. Filter by year, cause (partial match), sex or race/ethnicity.

NYC leading causes of death, by year, sex and race/ethnicity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Health & Water Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find flu vaccination sites in Manhattan that accept walk-ins."

**🤖 AI Agent:**
> list_flu_vaccination_sites with borough: "Manhattan" and walk_in: "Yes" returns the seasonal sites; borough matching is case-insensitive, so "manhattan" works too.

---

**👤 You:**
> "What were the leading causes of death in NYC in 2021?"

**🤖 AI Agent:**
> search_leading_causes_of_death with year: "2021" returns the leading causes with deaths, death rate and age-adjusted rate, broken down by sex and race/ethnicity; leading_cause narrows to one cause.

---

**👤 You:**
> "Show the per-capita water consumption trend in New York City."

**🤖 AI Agent:**
> get_water_consumption_trends returns one row per year with the city population, total consumption in million gallons per day and per-capita gallons per person per day; pass year to pin a single year.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How current is the water quality data?**
Distribution monitoring samples have run since 2015, so the search tools apply a 365-day sample-date window by default; pass after (and optionally an earlier before boundary) to widen or shift it. The annual water-consumption table is small — a few dozen rows, one per year.

**Q: What years do the causes-of-death statistics cover?**
Years 2007–2021, broken down by sex and race/ethnicity. search_leading_causes_of_death filters by year, cause (partial match), sex or race/ethnicity and returns deaths, death rate and the age-adjusted death rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-health-water-quality](https://vinkius.com/en/ai-agent-connect/nyc-health-water-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Health & Water Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-health-water-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Health & Water Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-health-water-quality": {
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
