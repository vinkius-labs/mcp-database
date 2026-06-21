# Tomorrow.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomorrowio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Equip your agent with precise weather intelligence, hyperlocal forecasts, and extreme climate risk assessments.

## Description
Connect your **Tomorrow.io** account to any AI agent and integrate institutional-grade weather modeling into your logic flows. Retrieve hyperlocal conditions, predict rainfall down to the specific minute, and access specialized environmental matrices (air quality, fire risks, and ground road weather) directly through natural language queries.

### What you can do

- **Real-time Observations** — Check comprehensive atmospheric indicators for any latitude, longitude, city, or zip code dynamically
- **Interval Forecasting** — Read forward-looking timelines segmented by minute (precipitation), hours (daily events), or deep daily projections up to 15 days out
- **Environmental Hazards** — Interrogate the AQI (Air Quality Index), pollen density predictions, or active Wildfire index algorithms
- **Logistical Safeguards** — Check specialized `Road Risk` parameters natively, enabling safer fleet routing algorithms against complex weather patterns
- **Historical Auditing** — Query observed historical conditions by defining past temporal boundaries and desired weather field sets for retroactive analysis

### How it works

1. Subscribe to this weather connector
2. Introduce your developer API Key located in your Tomorrow.io admin center
3. Engage your agent inquiring about global regions or embedding risk formulas locally

### Who is this for?

- **Data Engineers** — Fuse historical weather outcomes against localized internal databases directly via their programmatic environment
- **Fleet Operations Planners** — Assess "road risks" dynamically around routes and modify delivery paths automatically
- **Analytics Teams** — Predict attendance or consumer patterns merging upcoming precipitation and high-pollen counts with event data


## Available Tools (10)
- **get_air_quality_index**: Retrieve current and forecast air quality data
- **get_custom_timelines**: Query weather data for custom time ranges and arbitrary intervals
- **get_daily_forecast**: Returns up to 15 days of daily intervals.

Retrieve daily weather forecast extremes and totals
- **get_wildfire_risk**: Retrieve wildfire risk index and weather conditions
- **get_historical_weather**: Retrieve actual recorded historical weather observations
- **get_hourly_forecast**: Returns up to 120 hours of predictions.

Retrieve hour-by-hour weather forecast for a location
- **get_minutely_precipitation**: Retrieve minute-by-minute precipitation nowcast
- **get_pollen_forecast**: Retrieve daily pollen count indices
- **get_realtime_weather**: Provide a location (lat,lon, city name, or zip) and field list.

Retrieve current real-time weather conditions for any global location
- **get_road_weather_risk**: Retrieve assessments for driving and road hazards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tomorrow.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected air quality index in New York over the next hour?"

**🤖 AI Agent:**
> Based on the air quality data, the EPA Index for New York over the next hour is expected to be around '38', with the primary pollutant categorized as Fine Particulate Matter (PM2.5). The health concern reads as 'Good'.

---

**👤 You:**
> "Show me the minute-by-minute precipitation near Golden Gate bridge right now."

**🤖 AI Agent:**
> Over the next 60 minutes around the Golden Gate location, the predicted precipitation is registering strictly at 0.00 mm/hr continuously, indicating no expected rainfall directly matching those micro-coordinates.


## ❓ FAQ

**Q: Where do I retrieve my Tomorrow.io API Key?**
Log into your account via `app.tomorrow.io`. Navigate directly to the **API Management** or Developer tab nested inside your settings. Create a new root token, copy it in its entirety, and insert it securely to enable queries.

**Q: How accurate is the 'minutely' precipitation forecast tool?**
Tomorrow.io operates proprietary radar networks, satellites, and sophisticated high-resolution systems natively intended to provide powerful precision for up to exactly 60 minutes ahead, projecting precipitation downshifts incredibly well locally.

**Q: How far into the future can the agent forecast extreme weather events?**
Using Tomorrow.io's advanced predictive modeling, the agent can provide precise hour-by-hour projections and daily forecasts up to 15 days ahead. This extended timeline offers ample opportunity for logistical and operational planning against severe environmental risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomorrowio](https://vinkius.com/mcp/tomorrowio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tomorrow.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tomorrowio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tomorrow.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tomorrowio": {
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
