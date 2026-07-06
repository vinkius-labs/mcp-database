# Meteostat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meteostat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access historical weather data and climate statistics from thousands of weather stations and geographic points worldwide.

## Description
Connect to **Meteostat** to empower your AI agent with one of the largest databases of historical weather and climate data. Whether you need to analyze past weather patterns for a specific city or interpolate data for a remote coordinate, this server provides the tools to fetch precise meteorological records.

### What you can do

- **Station Discovery** — Use `stations_nearby` to find weather stations based on GPS coordinates and radius.
- **Historical Observations** — Fetch hourly, daily, or monthly data using `stations_hourly`, `stations_daily`, or `stations_monthly` for specific stations.
- **Point Interpolation** — Get weather data for any location on Earth, even without a local station, using `point_hourly` and `point_daily` tools.
- **Climate Normals** — Access long-term averages (30-year periods) via `stations_normals` to understand regional climate baselines.
- **Metadata & Search** — Retrieve detailed station information including WMO and ICAO identifiers using `stations_meta`.

### How it works

1. Subscribe to this server
2. Enter your Meteostat RapidAPI Key
3. Start querying weather history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — quickly pull historical weather datasets for environmental analysis or machine learning models.
- **Travel & Logistics Planners** — check historical weather patterns for specific dates and locations to optimize routing or event planning.
- **Developers** — integrate weather context into applications without building complex scrapers or data pipelines.


## Available Tools (10)
- **point_monthly**: Get historical monthly point data
- **point_normals**: Get climate normals for a point location
- **stations_daily**: Max 10 years per request.

Get historical daily statistics for a station
- **stations_hourly**: Max 30 days per request.

Get historical hourly observations for a station
- **stations_meta**: Specify at least one identifier (id, wmo, or icao).

Get metadata for a specific weather station
- **stations_monthly**: Get historical monthly statistics for a station
- **stations_nearby**: Find nearby weather stations by geo location
- **stations_normals**: Get climate normals for a station
- **point_daily**: Get historical daily point data
- **point_hourly**: Get historical hourly point data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meteostat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find weather stations within 20km of Lisbon (38.7, -9.1) using stations_nearby."

**🤖 AI Agent:**
> I found several stations near Lisbon. The closest is 'Lisboa / Geofisico' (ID: 08535) at 1.2km away, and 'Lisboa / Portela' (ID: 08536) at 6.5km. Which one should I pull data from?

---

**👤 You:**
> "What was the daily weather in New York (40.71, -74.00) during the first week of January 2023? Use point_daily."

**🤖 AI Agent:**
> Retrieving interpolated data for New York... During the first week of Jan 2023, temperatures ranged from a high of 14°C on Jan 4th to a low of 2°C on Jan 1st. There was light rain recorded on Jan 5th.

---

**👤 You:**
> "Get the 30-year climate normals for station 10637."

**🤖 AI Agent:**
> Fetching climate normals for station 10637 (Frankfurt am Main)... The average annual temperature is 10.6°C, with July being the warmest month (avg 20.1°C) and January the coldest (avg 1.6°C).


## ❓ FAQ

**Q: How can I find weather data for a location that doesn't have a specific weather station?**
You can use the `point_hourly` or `point_daily` tools. These tools use interpolation to calculate weather data for any geographic coordinate (latitude/longitude) by combining data from surrounding stations.

**Q: What is the difference between historical data and climate normals?**
Historical tools like `stations_daily` provide actual observations for specific dates. The `stations_normals` tool provides long-term statistical averages (usually over 30 years), which represent the 'typical' weather for a location.

**Q: Can I get weather data in Fahrenheit instead of Celsius?**
Yes. Most tools, such as `stations_hourly` and `point_daily`, include an optional `units` parameter. You can set this to 'imperial' to receive data in Fahrenheit and other non-metric units.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meteostat](https://vinkius.com/mcp/meteostat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meteostat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meteostat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meteostat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meteostat": {
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
