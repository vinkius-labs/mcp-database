# AerisWeather MCP Server

Access hyper-local weather data, forecasts, and alerts via AerisWeather — query observations, conditions, and geographical data directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aerisweather)

## Overview
**Category:** data-analytics
**Tools Count:** 6

## Description
Connect your **AerisWeather** account to any AI agent and access professional-grade weather intelligence through natural conversation.

### What you can do

- **Observations & Forecasts** — Fetch real-time METAR/PWS data and up to 15-day forecasts for any global location using `get_observations` and `get_forecasts`.
- **Global Conditions** — Get interpolated current, forecast, and historical weather conditions with minute-by-minute precipitation via `get_conditions`.
- **Weather Alerts** — Monitor active warnings, watches, and advisories from official sources like NWS and MeteoAlarm using `get_alerts`.
- **Geographical Data** — Retrieve detailed place information including timezones, population, and coordinates for cities or airports with `get_places`.
- **Batch Processing** — Efficiently query multiple endpoints in a single request to optimize agent performance using `get_batch`.

### How it works

1. Subscribe to this server
2. Enter your AerisWeather Client ID and Client Secret
3. Start querying weather data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Integrate weather context into applications or automation scripts directly from the IDE.
- **Logistics & Operations** — Monitor weather alerts and conditions for fleet management or event planning.
- **Data Analysts** — Access historical and real-time weather datasets for environmental research or business intelligence.


## Available Tools
- **get_alerts**: Get active weather warnings, watches, and advisories
- **get_batch**: Action is usually a location ID. Provide a comma-separated list of requests (e.g., /observations,/forecasts,/alerts). Max 31 requests.

Query multiple endpoints in a single request for efficiency
- **get_conditions**: Supports minutely precipitation forecasts (filter=minutelyprecip). Range: 2004 to +15 days.

Get interpolated global current, forecast, and historical conditions
- **get_forecasts**: Get weather forecasts
- **get_observations**: Action can be an ID (e.g., minneapolis,mn), closest, search, or within.

Get current weather observations
- **get_places**: Get geographical data for cities, stations, and airports


## Installation & Usage

To install and use the **AerisWeather** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aerisweather](https://vinkius.com/mcp/aerisweather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
