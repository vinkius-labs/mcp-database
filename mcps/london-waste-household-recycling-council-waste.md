# London Waste: Household Recycling & Council Waste MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/london-waste-household-recycling-council-waste)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless London waste data: household recycling rates by area (boroughs, London, England and the regions) from 2002/03, plus the council-waste annual split — landfill, incineration with and without energy recovery, recycling — London vs England, 2000/01 to 2024/25.

## Description
Two official London waste datasets — keyless, straight from the London open-data platform (data.london.gov.uk).

### What you can do
- **recycling_rates / recycling_rate_lookup / recycling_ranking / recycling_latest_year** — household recycling rates (% of household waste recycled) by area: the 33 London boroughs, London overall, England and the eight regions, on the 2002/03 onward series; a ranking of the areas on one year (best and worst sides) and the latest-year snapshot
- **waste_management_annual / waste_management_lookup / waste_management_overview** — the annual council-waste split per person: what percentage of London's (and England's) waste went to landfill, to incineration with energy recovery, to incineration without, to recycling, and what remained unrecycled, from 2000/01 to 2024/25; the overview returns the first year, the latest year and the deltas between them

### Who is this for
Urban policy researchers, sustainability teams and journalists comparing how London's waste mix has moved from landfill toward recycling. Years are stored as Excel serials in the source files; the tools map them to financial-year labels (2002/03 style, the UK fiscal year running April to March) so you filter by the label you see.


## Available Tools (7)
- **waste_management_annual**: Shares are fractions (0.5 = 50%). Optional financial year ("2024/25"). Page with limit/offset.

GLA annual waste-management indicators for London vs England
- **waste_management_lookup**: fy is required, e.g. "2024/25".

One year of the GLA waste-management indicators
- **waste_management_overview**: How London waste management changed, first vs last year
- **recycling_latest_year**: Latest published year of London household recycling rates
- **recycling_ranking**: All 43 published areas are compared (boroughs, City of London, Inner/Outer/London, regions, England). Optional top-N (max 43).

Rank London areas by household recycling rate
- **recycling_rate_lookup**: g. "Barnet", "London", "Inner London", "England"). area is required, matched case-insensitively.

Full recycling-rate time series for one area
- **recycling_rates**: g. 0.456 = 45.6%) by financial year from 2002/03 to 2024/25 (2011/12 is not published). Areas include the 33 London boroughs, City of London, Inner/Outer/London aggregates, the surrounding regions and England. Optional area (exact, case-insensitive) and year ("2024/25"). Page with limit/offset.

London household recycling rates by area and financial year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **London Waste: Household Recycling & Council Waste** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is London's household recycling rate in 2024/25?"

**🤖 AI Agent:**
> Call recycling_rate_lookup with area "London" and year "2024/25" — one rate for the whole city; recycling_ranking shows where London sits against England and the regions.

---

**👤 You:**
> "Which London boroughs recycle the least?"

**🤖 AI Agent:**
> Run recycling_ranking for the latest year — the bottom of the ranking lists the boroughs with the lowest household recycling rates, with the best side alongside.

---

**👤 You:**
> "How has London's landfilling changed since 2000?"

**🤖 AI Agent:**
> Call waste_management_overview — it returns the 2000/01 year, the 2024/25 year and the deltas: London's landfill share falls sharply over the series while the recycling share climbs.


## ❓ FAQ

**Q: Do I need an API key?**
No. data.london.gov.uk publishes every dataset as an anonymous file download (CSV or Excel). This MCP defines no credentials and needs nothing configured.

**Q: What is a financial year label like "2024/25"?**
The UK fiscal year runs April to March, so 2024/25 covers 1 April 2024 to 31 March 2025. The source files store years as Excel serial numbers; the tools convert them to these labels and accept the labels back as filters.

**Q: What do the waste fractions mean?**
The annual table is per resident: the share of all council-collected waste, in tonnes per person, that went to each route — landfill, incineration with energy recovery (EfW), incineration without, recycling, or nothing. The columns are London alongside England for the same year.

**Q: Do the recycling rates include the regions of England?**
Yes. The household recycling-rate series carries the 33 London boroughs, London overall, England and the eight English regions, so a ranking or lookup can name any of them — 'South East', 'London', 'Barnet', and so on.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/london-waste-household-recycling-council-waste](https://vinkius.com/en/ai-agent-connect/london-waste-household-recycling-council-waste)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **London Waste: Household Recycling & Council Waste** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `london-waste-household-recycling-council-waste` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **London Waste: Household Recycling & Council Waste** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "london-waste-household-recycling-council-waste": {
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
