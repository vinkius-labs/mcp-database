# Moscow Air, Weather & Green Spaces MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-air-weather-green-spaces)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [climate](../categories/climate.md)

Keyless Moscow environment: live air quality and its band, hourly air and weather forecasts, ERA5 monthly climate normals, parks and rivers.

## Description
What Moscow’s air, sky and green spaces are doing, keyless. The city’s monitoring portal is not openly reachable, so air data comes from Open-Meteo and the map from OpenStreetMap.

### What you can do
- **current_air_quality** — live PM2.5, PM10, CO, NO₂, O₃, SO₂ in µg/m³ plus the US AQI and its plain-language band
- **air_quality_forecast** — hourly PM2.5, PM10 and US AQI for the next hours (up to 168), in Europe/Moscow time
- **weather_forecast** — daily forecast up to 16 days: day/night temperature, precipitation, wind, UV, sunrise and sunset
- **seasonal_climate** — what the climate actually did in one year: ERA5 daily data collapsed into per-month averages, 1940–2025
- **park_inventory** — the mapped parks, gardens and groves (about 2,000), filterable by name or proximity
- **water_bodies** — rivers (Moskva, Yauza, Setun), ponds and reservoirs — about 1,800 reaches and 12,000 water areas

### Who is this for
Anyone planning outdoor time in Moscow: a run in a park, a day-trip forecast, or a packing list built on what the climate actually does.


## Available Tools (6)
- **air_quality_forecast**: 5, PM10 and the US AQI for the next hours — useful for planning outdoor time ("when does the air clear today"). Hours default to 24 and cap at 168 (a full week). The series is in Europe/Moscow local time.

Hourly air-quality forecast for Moscow
- **current_air_quality**: Returns the current PM2.5, PM10, carbon monoxide, nitrogen dioxide, ozone and sulphur dioxide in µg/m³ plus the US AQI and its plain-language band. Coordinates default to the city centre (55.7558, 37.6173); pass lat/lon for a district.

Current air quality in Moscow
- **park_inventory**: Each row carries the name, the green-space type (park, garden, recreation ground, nature reserve) and the centre coordinate. Filter by name fragment (Russian or English, e.g. "Парк Горького", "Sokolniki") or by proximity to a point. Parks with no mapped name are skipped by the name filter only.

Find parks and green spaces in Moscow
- **seasonal_climate**: Year defaults to 2025 (the last complete year) and may be any year from 1940 to 2025. Use it for "how cold is January in Moscow", "which month rains most", packing and season planning.

Monthly climate normals for Moscow (ERA5)
- **water_bodies**: Filter by name fragment (e.g. "Москва-река", "Яуза", "Нескучный") or by proximity to a point. Rivers are returned as reaches (way) with their centre coordinate.

Find rivers and water bodies in Moscow
- **weather_forecast**: Forecast length defaults to 7 days and caps at 16. Times are Europe/Moscow.

Daily weather forecast for Moscow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Air, Weather & Green Spaces** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the air in Moscow OK to run in right now?"

**🤖 AI Agent:**
> current_air_quality returns the live US AQI and its band; if it is Moderate or worse, air_quality_forecast shows when it clears.

---

**👤 You:**
> "How cold is January in Moscow, really?"

**🤖 AI Agent:**
> seasonal_climate with year 2025 collapses ERA5 daily data into per-month means, minima and maxima, plus precipitation and snowfall.

---

**👤 You:**
> "Find a park near Gorky Park."

**🤖 AI Agent:**
> park_inventory with lat/lon of Gorky Park (55.7290, 37.6050) and km 2 lists the green spaces around it; add a name fragment to narrow.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: Whose air-quality numbers are these?**
Open-Meteo’s air-quality API (a CAMS/forecast blend) for the coordinate you pass. It is not the city’s own monitoring network — that portal is not openly reachable from outside Russia.

**Q: How far back can the climate data go?**
The ERA5 reanalysis covers 1940 to 2025. Pass year to summarise any of them; the default is 2025, the last complete year.

**Q: Can I search parks near a point?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Use it before a long list — a citywide scan is heavy and capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-air-weather-green-spaces](https://vinkius.com/en/ai-agent-connect/moscow-air-weather-green-spaces)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Air, Weather & Green Spaces** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-air-weather-green-spaces` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Air, Weather & Green Spaces** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-air-weather-green-spaces": {
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
