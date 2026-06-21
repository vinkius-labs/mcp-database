# NOAA Forecast — US Weather Predictions MCP Server

Official NWS weather forecasts for any US location: 7-day daily forecasts, 156-hour hourly forecasts, raw grid data, and meteorologist forecast discussions from 122 Weather Forecast Offices.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/noaa-forecast-us-weather-predictions)

## Overview
**Category:** the-unthinkable
**Tools Count:** 5

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


## Installation & Usage

To install and use the **NOAA Forecast — US Weather Predictions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/noaa-forecast-us-weather-predictions](https://vinkius.com/mcp/noaa-forecast-us-weather-predictions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
