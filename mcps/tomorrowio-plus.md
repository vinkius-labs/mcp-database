# Tomorrow.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomorrowio-plus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tomorrowio-plus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tomorrowio-plus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access hyper-local weather data, real-time conditions, forecasts, and historical weather directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tomorrow.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current temperature and humidity in London?"

**🤖 AI Agent:**
> I'll check the real-time weather for London... The current temperature is 15°C with 72% humidity and clear skies.

---

**👤 You:**
> "Show me the daily forecast for the next 3 days at coordinates [40.71, -74.00]."

**🤖 AI Agent:**
> Fetching the 3-day forecast... Tomorrow expects light rain, followed by two sunny days with highs around 22°C.

---

**👤 You:**
> "List all active weather alerts for my saved locations."

**🤖 AI Agent:**
> Checking for alerts... I found one active High Wind Warning for your 'East Coast Warehouse' location valid until 6 PM tonight.


## Installation & Usage

To install and use the **Tomorrow.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomorrowio-plus](https://vinkius.com/mcp/tomorrowio-plus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
