# Open-Meteo Full Access MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-full-access)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

The ultimate weather Mega-Server: 15 tools covering forecast, historical (84 years), marine, air quality, pollen, climate projections (to 2100), flood, geocoding, and elevation — all in one zero-auth integration.

## Description
The **definitive Mega-Server** for weather and climate intelligence. Why install 7 servers when one does it all?

### What you can do
- **Live Weather** — 16-day forecast + current conditions for any GPS coordinate
- **84 Years of History** — Hourly weather archives from 1940 to today
- **Ocean Intelligence** — Wave height, swell, currents, sea surface temperature at 5km
- **Air Safety** — PM2.5, PM10, O₃, pollen counts, European & US AQI
- **Climate Future** — IPCC projections to 2100 + ensemble probabilistic forecasts
- **Flood Risk** — GloFAS river discharge with 40 years of reanalysis + 7 months forward
- **Location Tools** — Global geocoding and 90m terrain elevation

### Who is this for?
Power users, data scientists, multi-disciplinary analysts, and anyone building the most capable weather-aware AI agent imaginable.


## Available Tools (15)
- **get_weather_forecast**: Get weather forecast for any location (up to 16 days)
- **get_climate_projection**: Get IPCC climate projections (2015–2100)
- **get_ensemble_forecast**: Get probabilistic multi-model ensemble forecast
- **get_river_discharge**: Get river discharge data at 5km resolution
- **get_flood_forecast**: Get flood forecast up to 7 months ahead
- **search_location**: Search cities and locations globally
- **get_elevation**: Get terrain elevation for any coordinates
- **get_current_weather**: Get current weather conditions
- **get_historical_weather**: Covers 84 years.

Get historical weather (1940–present)
- **get_historical_daily**: Get historical daily aggregates
- **get_marine_forecast**: Get marine wave forecast at 5km resolution
- **get_ocean_currents**: Get ocean currents and sea surface temperature
- **get_air_quality**: 5, PM10, ozone, NO2, SO2, CO concentrations.

Get air quality pollutant concentrations
- **get_aqi_index**: Get AQI (European and US standards)
- **get_pollen_forecast**: Get pollen and allergen forecast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Full Access** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full weather briefing for a yacht trip from Lisbon to Madeira next week"

**🤖 AI Agent:**
> ⛵ **Lisbon → Madeira Full Briefing**

🌤️ Forecast: 22-25°C, partly cloudy, light rain Day 3
🌊 Waves: 1.5-2.2m, SW swell, period 10s
💨 Air Quality: AQI 35 (Good) both endpoints
🏞️ Elevation: Departure 0m → Arrival 0m (sea level)
📍 Route: 38.72°N → 32.65°N (978km)

Favorable conditions overall. Day 3 requires attention.

---

**👤 You:**
> "Climate risk assessment for a new data center in Singapore"

**🤖 AI Agent:**
> 🏢 **Singapore — Climate Risk Assessment**

🌡️ Current avg: 27.5°C → 2060 projected: 29.8°C
🌊 Flood risk: Moderate (river discharge 45 m³/s, seasonal peaks)
💨 Air quality: AQI varies 30-150 (haze season Sep-Oct)
🌧️ Historical rain: avg 2,340mm/year, increasing trend

Key risks: Rising cooling costs, seasonal haze, flash flood exposure.

---

**👤 You:**
> "What was the weather like on the day I was born? July 15, 1990 in Rome"

**🤖 AI Agent:**
> 🎂 **Rome — July 15, 1990**

Max temp: 34.2°C | Min: 21.8°C
Sunshine: 13.5 hours
Precipitation: 0mm (perfectly dry)
Wind: 8 km/h from the south

You were born on a beautiful, hot Roman summer day! ☀️


## ❓ FAQ

**Q: Why choose the Full server instead of individual ones?**
The Full server bundles **all 15 tools** from all 7 domain-specific servers into a single integration. Perfect for multi-disciplinary AI agents that need weather, climate, marine, air quality, flood, and location data without managing multiple connections.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-full-access](https://vinkius.com/mcp/open-meteo-full-access)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open-Meteo Full Access** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-meteo-full-access` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open-Meteo Full Access** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-meteo-full-access": {
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
