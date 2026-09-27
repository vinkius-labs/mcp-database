# NYC Climate, Emissions & Environmental Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-climate-emissions-environmental-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC climate and environment data: citywide and municipal greenhouse-gas inventories, heat-vulnerability by ZIP+4, rooftop solar sites, street-level flood events, climate projections and air-quality sensor readings — no API key.

## Description
Official city climate, emissions and public-environment records, keyless, for analysis and verification.

### What you can do
- **GHG inventories** — citywide sector-by-sector emissions or the city government's own footprint, year by year (2005–2024)
- **Heat vulnerability** — the heat-vulnerability index by ZIP+4 area; rank the most vulnerable neighborhoods
- **Rooftop solar** — agency and community solar sites with borough and project status
- **Street flooding** — sensor-recorded inundation events with start time and maximum water depth
- **Climate projections** — temperature and precipitation scenarios per model period
- **Air quality** — sensor readings (e.g. PM2.5) with period start dates

### Who is this for
Environmental analysis, urban-resilience planning, journalism and any agent that must verify a climate or emissions claim against official city records.


## Available Tools (6)
- **get_climate_projections**: period values look like "2030s (25th Percentile)", "2050s (75th Percentile)", "2150 (90th Percentile)" — each period has one row with all the metrics.

NYC climate projection metrics for one future period
- **get_ghg_inventory**: scope "citywide" is the whole-city inventory (2005-2024); scope "municipal" is city government operations only (2006-2024). Narrow with the sector parameter; the CO2e column is resolved automatically for the chosen year.

NYC greenhouse gas inventory emissions for one year (citywide or municipal)
- **list_flood_events**: Filter by sensor name or a start-time window. These are measured street-flood events, not storm drains.

FloodNet sensor flood events (street flooding readings)
- **rank_heat_vulnerability**: Without zcta, returns the top N most vulnerable areas; with zcta, returns that one area's rank. Use it to contextualize heat-related questions (e.g. which neighborhoods need the most cooling resources).

Heat Vulnerability Index ranking of ZIP+4 areas (ZCTAs)
- **search_aq_sensor_readings**: 5 readings from the Queens air-quality sensor pilot: each row is one period's mean PM2.5 mass concentration and the US EPA nowcast AQI, with the sensor's lat/lon. Filter by sensor id or a start-of-period window. This is a pilot network, not the full city AQ picture.

PM2.5 air quality sensor readings (Queens pilot network)
- **search_solar_sites**: Filter by borough, agency (site owner type), council district or status.

Search the NYC Solar Readiness project sites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Climate, Emissions & Environmental Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much CO2 does the city government emit in 2024?"

**🤖 AI Agent:**
> get_ghg_inventory with scope "municipal" and year "2024" returns the government's own footprint split by main sector.

---

**👤 You:**
> "Which ZIP codes face the most heat risk?"

**🤖 AI Agent:**
> rank_heat_vulnerability without a zcta returns the most exposed ZIP+4 areas citywide (optionally by borough); pass a zcta to pull the index for one specific area.

---

**👤 You:**
> "Has this area flooded recently?"

**🤖 AI Agent:**
> list_flood_events with start_after a recent date returns the sensor-recorded inundation events since then, with start times and maximum water depth.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: What does the GHG tool return?**
For one year you get the emissions split: citywide mode gives sector-by-sector tonnes of CO2-equivalent across the whole city; municipal mode gives the city government's own footprint by main sector. Years run from 2005 to 2024.

**Q: How is heat vulnerability ranked?**
Each ZIP+4 area carries a heat-vulnerability index where the higher the value, the more exposed the residents are. With a ZIP+4 the tool returns that one area; without it, the top-N most vulnerable areas in the chosen borough.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-climate-emissions-environmental-data](https://vinkius.com/en/ai-agent-connect/nyc-climate-emissions-environmental-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Climate, Emissions & Environmental Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-climate-emissions-environmental-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Climate, Emissions & Environmental Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-climate-emissions-environmental-data": {
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
