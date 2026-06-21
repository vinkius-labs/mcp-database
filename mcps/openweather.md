# OpenWeather MCP Server

Get weather data worldwide — current conditions, forecasts, air quality, alerts and historical data from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openweather)

## Overview
**Category:** iot-hardware
**Tools Count:** 11

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


## Available Tools
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


## Installation & Usage

To install and use the **OpenWeather** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openweather](https://vinkius.com/mcp/openweather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
