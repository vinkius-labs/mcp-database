# Weatherbit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weatherbit-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/weatherbit-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/weatherbit-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time weather data, 16-day forecasts, air quality metrics, and severe weather alerts globally.

## Description
Connect **Weatherbit** to your AI agent to retrieve hyper-local weather intelligence. From 16-day forecasts to real-time lightning strikes and air quality metrics, this server provides the environmental context your agent needs.

### What you can do

- **Current Conditions** — Get real-time observations including temperature, wind, and precipitation via `get_current_weather`.
- **Forecasts** — Access 16-day daily, 10-day hourly, and 60-minute precipitation forecasts using `get_daily_forecast`, `get_hourly_forecast`, and `get_minutely_forecast`.
- **Air Quality** — Monitor current and 3-day forecasted air quality (AQI, PM2.5, etc.) with `get_current_airquality` and `get_airquality_forecast`.
- **Severe Weather** — Fetch active weather alerts from local agencies via `get_alerts`.
- **Lightning Tracking** — Locate the nearest lightning strikes with precise coordinates using `get_current_lightning`.

### How it works

1. Subscribe to this server
2. Enter your Weatherbit API Key
3. Query weather data directly from Claude, Cursor, or any MCP-compatible client.


## Available Tools
- **get_airquality_forecast**: Requires lat and lon.

Get 3-day hourly air quality forecast
- **get_alerts**: Provide lat/lon OR city OR postal_code OR city_id.

Get severe weather alerts
- **get_current_airquality**: 5, PM10, CO, SO2, NO2, O3) and AQI. Provide lat/lon OR city OR postal_code OR city_id.

Get current air quality
- **get_current_lightning**: Requires lat and lon.

Get nearest lightning observations
- **get_current_weather**: Provide lat/lon OR city OR postal_code OR city_id OR station.

Get current weather observations
- **get_daily_forecast**: Provide lat/lon OR city OR postal_code OR city_id.

Get 16-day daily forecast
- **get_daily_history**: Requires lat, lon, start_date, end_date (YYYY-MM-DD).

Get daily historical weather
- **get_geocode**: Provide city OR postal_code OR city_id OR station.

Geocoding API
- **get_hourly_forecast**: Requires lat and lon.

Get up to 10-day hourly forecast
- **get_hourly_history**: Requires lat, lon, start_date, end_date (YYYY-MM-DD:HH).

Get hourly historical weather
- **get_minutely_forecast**: Requires lat and lon.

Get 1-hour minutely precipitation forecast
- **get_normals**: Requires lat, lon, start_day, end_day (MM-DD).

Get climate normals (1991-2020)
- **get_subhourly_history**: Requires lat, lon, start_date, end_date.

Get sub-hourly historical weather
- **get_subscription_usage**: Get subscription usage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weatherbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current weather and air quality in Tokyo?"

**🤖 AI Agent:**
> In Tokyo, it's currently 18°C with clear skies. The Air Quality Index (AQI) is 42, which is considered Good.

---

**👤 You:**
> "Check for any severe weather alerts in Paris."

**🤖 AI Agent:**
> I've checked the local agencies for Paris. There is currently a Yellow Alert for heavy rainfall expected this evening.

---

**👤 You:**
> "Give me a 16-day daily forecast for Berlin."

**🤖 AI Agent:**
> Fetching the 16-day outlook for Berlin... Temperatures will range from 10°C to 15°C over the next week with intermittent showers starting Wednesday.


## Installation & Usage

To install and use the **Weatherbit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weatherbit-alternative](https://vinkius.com/mcp/weatherbit-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
