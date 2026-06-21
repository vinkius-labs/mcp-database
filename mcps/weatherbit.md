# Weatherbit MCP Server

Get real-time weather, forecasts, historical data, severe alerts and air quality for any location worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/weatherbit)

## Overview
**Category:** data-analytics
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Weatherbit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weatherbit](https://vinkius.com/mcp/weatherbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
