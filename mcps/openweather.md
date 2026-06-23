# OpenWeather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openweather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Get weather data worldwide — current conditions, forecasts, air quality, alerts and historical data from any AI agent.

## Description
Connect to **OpenWeather** APIs and access global weather data through natural conversation.

### What you can do

- **Current Weather** — Get real-time temperature, humidity, wind, pressure, visibility and conditions for any location
- **Hourly Forecast** — 48-hour hourly forecast with temperature, precipitation probability and UV index
- **Daily Forecast** — Up to 16-day daily forecast with min/max temperatures and weather descriptions
- **Weather Alerts** — Active severe weather warnings and alerts for any location
- **Air Quality** — Current AQI and 4-day forecast with pollutant concentrations (PM2.5, PM10, O3, NO2, CO)
- **Historical Weather** — Weather conditions for any past date
- **Sun Times** — Sunrise and sunset times for any location
- **Geocoding** — Convert city names to coordinates and vice versa

### How it works

1. Subscribe to this server
2. Enter your OpenWeather API Key
3. Start exploring weather data from Claude, Cursor, or any MCP-compatible client

No more checking weather apps — just ask your AI.

### Who is this for?

- **Travelers** — check weather forecasts and alerts before and during trips
- **Event Planners** — monitor weather conditions and UV index for outdoor events
- **Outdoor Enthusiasts** — check sunrise/sunset times, air quality and hourly forecasts
- **Researchers** — access historical weather data and air quality trends


## Available Tools (11)
- **geocode**: Returns the top 5 matching locations with their coordinates, country codes and state names. Use these coordinates with other weather tools.

Convert a city name to coordinates
- **get_air_quality**: 5, PM10, O3, NO2, SO2, CO, NH3). AQI scale: 1=Good, 2=Fair, 3=Moderate, 4=Poor, 5=Very Poor. Requires lat/lon coordinates.

Get current air quality index for a location
- **get_air_quality_forecast**: Each data point includes AQI level (1-5 scale) and concentrations of PM2.5, PM10, O3, NO2, SO2, CO and NH3.

Get 4-day air quality forecast for a location
- **get_forecast**: Each data point includes temperature, humidity, wind, pressure and weather description. Optionally set the number of days (1-5). Requires either city name or lat/lon.

Get 5-day/3-hour weather forecast
- **get_historical_weather**: Returns temperature, humidity, wind, pressure and weather description for the requested date. Requires lat/lon and date in YYYY-MM-DD format.

Get historical weather data for a specific date
- **get_current_weather**: Requires either city name (e.g. "London", "São Paulo") or latitude/longitude coordinates.

Get current weather conditions for a location
- **get_daily_forecast**: Each day includes min/max temperature, humidity, wind, UV index, precipitation probability and weather description. Requires lat/lon coordinates.

Get daily weather forecast for up to 16 days
- **get_hourly_forecast**: Each hour includes temperature, humidity, wind, UV index, precipitation probability and weather description. Requires lat/lon coordinates. Use geocode to find coordinates for a city name.

Get hourly weather forecast using One Call API
- **get_sun_times**: Returns the exact times and the sun's elevation angle at sunrise/sunset. Requires lat/lon coordinates.

Get sunrise and sunset times for a location
- **get_weather_alerts**: Returns alert type, severity, description, start and end times. Requires lat/lon coordinates. Useful for monitoring severe weather conditions.

Get active weather alerts for a location
- **reverse_geocode**: Returns the city, state, country and postal code for the given coordinates.

Convert coordinates to a city name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenWeather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current weather in São Paulo?"

**🤖 AI Agent:**
> São Paulo is currently 24°C (75°F), partly cloudy. Humidity: 65%, Wind: 12 km/h SE, Pressure: 1013 hPa, Visibility: 10 km. Feels like 25°C. Sunrise at 6:12 AM, sunset at 6:45 PM.

---

**👤 You:**
> "What's the 7-day forecast for Tokyo?"

**🤖 AI Agent:**
> 7-day forecast for Tokyo: Mon 22°C/15°C (rain), Tue 19°C/14°C (cloudy), Wed 21°C/16°C (partly cloudy), Thu 23°C/17°C (sunny), Fri 24°C/18°C (sunny), Sat 22°C/17°C (light rain), Sun 20°C/15°C (overcast).

---

**👤 You:**
> "Is the air quality good in Beijing right now?"

**🤖 AI Agent:**
> Beijing's current AQI is 4 (Poor). PM2.5 is 75 μg/m³ (3x WHO guideline), PM10 is 120 μg/m³. Ozone and NO2 levels are moderate. Sensitive groups should reduce outdoor exposure.


## ❓ FAQ

**Q: How do I get an OpenWeather API key?**
Visit [**openweathermap.org/api**](https://openweathermap.org/api), click **Sign Up** for a free account, go to **API Keys** in your account settings, and create a new key. Copy it — it's a 32-character hex string. Free tier includes 60 calls/minute.

**Q: Can I get weather alerts for my location?**
Yes! Use `get_weather_alerts` with lat/lon coordinates. Returns active alerts with sender name, event type, severity, description and start/end times. Useful for monitoring severe weather, floods, heat waves and other dangerous conditions.

**Q: Can I get historical weather data?**
Yes! Use `get_historical_weather` with lat/lon and a date in YYYY-MM-DD format. Returns the weather conditions for that specific day including temperature, humidity, wind and pressure.

**Q: How do I find coordinates for a city?**
Use `geocode` with the city name (e.g. 'London', 'São Paulo', 'Tokyo'). Returns the top 5 matching locations with their latitude, longitude, country code and state. Use these coordinates with other weather tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openweather](https://vinkius.com/mcp/openweather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenWeather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openweather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenWeather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openweather": {
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
