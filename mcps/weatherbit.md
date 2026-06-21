# Weatherbit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weatherbit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/weatherbit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/weatherbit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Get real-time weather, forecasts, historical data, severe alerts and air quality for any location worldwide.

## Description
Connect to **Weatherbit** and access global weather data through natural conversation.

### What you can do

- **Current Weather** — Get real-time conditions (temperature, humidity, wind, precipitation, UV) by coordinates or city name
- **Daily Forecast** — Get up to 16-day daily forecasts with high/low temps, precipitation, wind and UV
- **Hourly Forecast** — Get up to 10-day hourly forecasts with detailed conditions
- **Historical Weather** — Access 30+ years of historical daily weather data
- **Weather Alerts** — Get active severe weather warnings and watches
- **Air Quality** — Get AQI, PM2.5, PM10, O3, NO2, SO2 and CO readings
- **Severe Weather** — Query recent severe weather reports (tornadoes, hail, floods)

### How it works

1. Subscribe to this server
2. Enter your Weatherbit API Key (free: 500 calls/day)
3. Start exploring weather data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travelers** — check forecasts before trips and monitor weather at destination
- **Outdoor Workers** — get accurate forecasts and severe weather alerts for planning
- **Researchers** — access historical weather data for climate and agricultural analysis


## Available Tools
- **get_air_quality**: Returns AQI score, PM2.5, PM10, O3, NO2, SO2, CO concentrations and health recommendations.

Get air quality index (AQI) by coordinates
- **get_current_weather**: Returns temperature, feels like, humidity, wind speed/direction, precipitation, cloud cover, visibility, UV index, weather description and icon.

Get current weather conditions by coordinates
- **get_current_weather_by_city**: Returns temperature, feels like, humidity, wind, precipitation, cloud cover, visibility, UV index and weather description.

Get current weather conditions by city name
- **get_forecast_daily**: Returns daily high/low temperatures, weather conditions, precipitation probability, wind, humidity, UV index and sunrise/sunset times.

Get daily weather forecast by coordinates
- **get_forecast_daily_by_city**: Returns daily forecasts for up to 16 days ahead with temperatures, conditions, precipitation, wind and UV index.

Get daily weather forecast by city name
- **get_forecast_hourly**: Returns temperature, precipitation probability, wind, humidity, cloud cover and weather conditions for each hour.

Get hourly weather forecast by coordinates
- **get_forecast_hourly_by_city**: Returns hourly forecasts with temperature, precipitation, wind and conditions.

Get hourly weather forecast by city name
- **get_historical_weather**: Returns temperature, precipitation, wind, humidity and other metrics for dates in the past 30 years.

Get historical weather data by coordinates
- **get_severe_weather**: Useful for tracking recent severe weather activity.

Query severe weather reports in a geographic area
- **get_weather_alerts**: Returns alert type, severity, description, effective/expiry times and affected areas.

Get active weather alerts by coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weatherbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather in London today?"

**🤖 AI Agent:**
> London: 15°C (feels 13°C), light rain, 78% humidity, wind 12 km/h NE. Cloud cover 85%. UV index 2 (low). Sunrise 06:42, Sunset 18:15.

---

**👤 You:**
> "Give me the 5-day forecast for Tokyo."

**🤖 AI Agent:**
> Tokyo 5-day forecast: Mon 22°C/14°C ☀️, Tue 20°C/13°C ⛅, Wed 18°C/12°C 🌧️, Thu 21°C/14°C ⛅, Fri 23°C/15°C ☀️.

---

**👤 You:**
> "What's the air quality in São Paulo?"

**🤖 AI Agent:**
> São Paulo AQI: 65 (Moderate). PM2.5: 19 μg/m³, PM10: 38 μg/m³, O3: 42 ppb. Sensitive groups should limit outdoor activity.


## Installation & Usage

To install and use the **Weatherbit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weatherbit](https://vinkius.com/mcp/weatherbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
