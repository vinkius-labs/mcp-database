# NOAA Forecast — US Weather Predictions MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-forecast-us-weather-predictions)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/noaa-forecast-us-weather-predictions-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/noaa-forecast-us-weather-predictions-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Official NWS weather forecasts for any US location: 7-day daily forecasts, 156-hour hourly forecasts, raw grid data, and meteorologist forecast discussions from 122 Weather Forecast Offices.

## Description
Connect your AI agent to the official National Weather Service forecast engine.

### What you can do
- **7-Day Forecast** — Daily forecast with highs, lows, precipitation, and detailed narrative
- **Hourly Forecast** — 156 hours of hour-by-hour conditions
- **Grid Data** — Raw quantitative arrays: temperature, precipitation, wind, humidity
- **Forecast Discussion** — Technical AFD from NWS meteorologists at 122 offices
- **Point Metadata** — WFO assignment, grid coordinates, zone info

### No API Key Required
Completely open. No registration needed.

### US Locations Only
The NWS API covers the United States, Puerto Rico, Guam, and US territories.


## Available Tools
- **get_forecast**: Provide latitude and longitude for any US location. Returns high/low temps, wind speed/direction, precipitation probability, and detailed narrative.

Get 7-day weather forecast for a US location by latitude and longitude
- **get_hourly_forecast**: 5 days. Includes temperature, wind, humidity, precipitation, and sky condition for each hour. US locations only.

Get hour-by-hour weather forecast (156 hours) for a US location
- **get_forecast_discussion**: Use the 3-letter WFO code (e.g., OKX=New York, LAX=Los Angeles, MFL=Miami). Lists recent product IDs — retrieve the latest for full text.

Get the Area Forecast Discussion (AFD) from a NWS Weather Forecast Office
- **get_grid_data**: Useful for programmatic analysis. US only.

Get raw NWS grid weather data: temperature, precipitation, wind, humidity arrays
- **get_point_metadata**: US locations only.

Get NWS metadata for a US location: responsible WFO, grid coordinates, zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NOAA Forecast — US Weather Predictions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather forecast for New York City this week?"

**🤖 AI Agent:**
> 🌤️ **NYC 7-Day Forecast**

Today: Partly cloudy, High 72°F, Wind SW 10 mph
Tonight: Clear, Low 58°F
Wednesday: Sunny, High 78°F
Thursday: Thunderstorms, High 74°F, 60% chance rain
Friday: Clearing, High 68°F
Weekend: Sunny, Highs 72-75°F

Source: NWS Office OKX (Upton, NY)

---

**👤 You:**
> "Get hourly forecast for Miami Beach"

**🤖 AI Agent:**
> ⏰ **Miami Beach — Hourly Forecast**

| Hour | Temp | Wind | Rain |
|------|------|------|------|
| 2pm | 88°F | SE 12 | 10% |
| 3pm | 89°F | SE 14 | 20% |
| 4pm | 87°F | SE 15 | 40% |
| 5pm | 84°F | S 18 | 60% |
| 6pm | 82°F | S 12 | 30% |

Afternoon sea-breeze thunderstorms likely.


## Installation & Usage

To install and use the **NOAA Forecast — US Weather Predictions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-forecast-us-weather-predictions](https://vinkius.com/mcp/noaa-forecast-us-weather-predictions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
