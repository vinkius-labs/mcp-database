# Open-Meteo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/open-meteo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/open-meteo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Get weather forecasts, historical data and air quality — no API key required, open-source weather data.

## Description
Connect to **Open-Meteo** and access global weather forecasts through natural conversation — no API key needed.

### What you can do

- **Current Weather** — Get real-time temperature, humidity, wind, precipitation and conditions
- **7-Day Forecast** — Hourly and daily forecasts up to 16 days ahead with 50+ weather variables
- **Historical Weather** — Access archived weather data going back to 1940 for any location
- **Air Quality** — Get PM2.5, PM10, NO2, O3, SO2, CO and UV index forecasts
- **Geocoding** — Find coordinates for any city or place name
- **Elevation** — Get elevation data for any coordinates

### How it works

1. Subscribe to this server
2. No API key needed — start querying immediately
3. Get weather data from Claude, Cursor, or any MCP-compatible client

No API key required — completely free and open-source.

### Who is this for?

- **Travelers** — check weather forecasts and air quality before and during trips
- **Researchers** — access historical weather data for climate studies and analysis
- **Developers** — integrate free weather data into applications without authentication
- **Outdoor Planners** — check UV index, wind speed and precipitation for events


## Available Tools
- **get_air_quality**: 5, PM10, nitrogen dioxide, ozone, sulphur dioxide, carbon monoxide, dust, pollen and UV index. Requires latitude and longitude. Returns hourly data for up to 7 days. Common variables: pm2_5, pm10, nitrogen_dioxide, ozone, sulphur_dioxide, carbon_monoxide, dust, uv_index, alder_pollen, grass_pollen.

Get air quality forecast for a location
- **get_elevation**: Useful for hiking, aviation and geographic research.

Get elevation for coordinates
- **get_forecast**: Requires latitude and longitude. Supports hourly, daily and current weather variables. Common variables: temperature_2m, relative_humidity_2m, precipitation, rain, snowfall, wind_speed_10m, wind_direction_10m, wind_gusts_10m, weather_code, cloud_cover, pressure_msl, uv_index, visibility, apparent_temperature, dew_point_2m, sunshine_duration. Set past_days to include historical data (0-92 days). Set forecast_days for forecast length (0-16 days, default 7). Timezone defaults to GMT; use "auto" for local timezone.

Get weather forecast for a location
- **get_geocoding**: Useful for finding coordinates to use with weather tools. Returns up to 10 results by default.

Find coordinates for a place name
- **get_historical_weather**: Requires latitude, longitude, start date and end date (YYYY-MM-DD format). Supports the same hourly variables as the forecast API. Historical data goes back to 1940 for most locations. Use get_geocoding to find coordinates for a city name.

Get historical weather data for a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather forecast for São Paulo this week?"

**🤖 AI Agent:**
> São Paulo (23.55°S, 46.63°W): Today 26°C/18°C, partly cloudy with 30% chance of rain. Tomorrow 24°C/17°C, light rain expected. Wednesday 22°C/16°C, overcast. Wind: 10-15 km/h. Humidity: 65-80%. UV index moderate (5-6).

---

**👤 You:**
> "What was the temperature in Tokyo on July 15, 2024?"

**🤖 AI Agent:**
> Tokyo on July 15, 2024: High 32°C, Low 25°C. Hourly data shows temperatures peaked at 2 PM. Humidity 70%, light winds 5 km/h from the southeast. No precipitation recorded.

---

**👤 You:**
> "What's the air quality in Beijing right now?"

**🤖 AI Agent:**
> Beijing air quality: PM2.5 at 85 μg/m³ (unhealthy for sensitive groups), PM10 at 120 μg/m³, NO2 at 45 μg/m³, O3 at 65 μg/m³. Overall AQI: 165 (Unhealthy). Sensitive groups should reduce outdoor exposure.


## Installation & Usage

To install and use the **Open-Meteo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo](https://vinkius.com/mcp/open-meteo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
