# Open-Meteo MCP Server

Get weather forecasts, historical data and air quality — no API key required, open-source weather data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo)

## Overview
**Category:** data-analytics
**Tools Count:** 5

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


## Installation & Usage

To install and use the **Open-Meteo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo](https://vinkius.com/mcp/open-meteo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
