# Tomorrow.io MCP Server

Access hyper-local weather data, real-time conditions, forecasts, and historical weather directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tomorrowio-plus)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Connect **Tomorrow.io** to your AI agent to leverage the world's most accurate weather intelligence. From hyper-local real-time conditions to complex GeoJSON-based timelines, this server provides everything needed for weather-dependent decision making.

### What you can do

- **Real-time & Forecasts** — Get current conditions or hourly/daily forecasts for any specific location or coordinate.
- **Weather Timelines** — Retrieve detailed timelines for specific fields like temperature, precipitation, wind speed, and more.
- **Historical Data** — Access weather history for the last 24 hours to analyze recent atmospheric trends.
- **Map Visualizations** — Fetch map tiles for weather layers to integrate visual data into mapping applications.
- **Alerts & Insights** — Monitor active weather alerts and predefined insight categories for proactive risk management.
- **Location Management** — List and manage saved locations for consistent monitoring across your organization.

### How it works

1. Subscribe to this server
2. Enter your Tomorrow.io API Key
3. Start querying weather data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Fleet Managers** — Optimize routes based on real-time weather conditions and active alerts.
- **Energy & Utility Providers** — Forecast demand and manage infrastructure risks with precise atmospheric data.
- **Developers** — Build weather-aware applications using simple natural language queries instead of complex API calls.


## Available Tools
- **list_alerts**: List all active weather alerts based on your insights and locations
- **list_events**: Retrieve specific weather events for a location based on insight categories
- **get_forecast_weather**: Retrieve hourly or daily weather forecasts
- **get_timelines**: Fields can be temperature, precipitationIntensity, etc.

Retrieve weather data for a specific location and time range
- **list_insights**: List all pre-defined or custom insight categories
- **list_locations**: List all pre-defined locations in your account
- **get_map_tile**: Retrieve weather map tiles for integration into mapping applications
- **post_timelines**: Retrieve weather data for complex location types like GeoJSON geometries
- **get_realtime_weather**: Retrieve current weather conditions for a location
- **get_recent_history_weather**: Retrieve weather history for the last 24 hours


## Installation & Usage

To install and use the **Tomorrow.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomorrowio-plus](https://vinkius.com/mcp/tomorrowio-plus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
