# AccuWeather MCP Server

Access real-time weather data, detailed forecasts, and location-based climate insights directly from your AI agent using AccuWeather's global network.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/accuweather-alternative)

## Overview
**Category:** data-analytics
**Tools Count:** 13

## Description
Connect your **AccuWeather** API to any AI agent to integrate hyper-local weather intelligence into your workflows. This server provides comprehensive access to the world's most accurate weather data.

### What you can do

- **Location Discovery** — Find location keys via city names (`search_city`), geographic coordinates (`search_geoposition`), or IP addresses (`search_ipaddress`).
- **Current Conditions** — Retrieve real-time weather data including temperature, humidity, and wind speed using `current_conditions` or look back with `historical_conditions`.
- **Detailed Forecasts** — Get precise daily (`daily_forecast`) or hourly (`hourly_forecast`) predictions to plan activities or automate weather-dependent tasks.
- **Advanced Metrics** — Access specialized data like `minutecast` for hyper-local precipitation or `lightning_radius` for safety monitoring.
- **Global Insights** — Query `top_cities` to get a snapshot of weather conditions across major global or regional hubs.

### How it works

1. Subscribe to this server
2. Enter your AccuWeather API Key
3. Start querying weather data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Travel** — Automate route planning based on hourly forecasts and weather alarms.
- **Developers** — Integrate weather context into applications without leaving the code editor.
- **Data Analysts** — Gather historical and current climate data for regional reporting.


## Available Tools
- **alarms**: Get weather-related alarms for a location key
- **autocomplete_city**: Get city suggestions as you type
- **current_conditions**: Get current weather conditions for a location key
- **daily_forecast**: Get daily weather forecasts for a location key
- **historical_conditions**: Get historical current conditions
- **hourly_forecast**: Get hourly weather forecasts for a location key
- **lightning_box**: Get lightning strike data within a bounding box
- **lightning_radius**: Get lightning strike data within a specific radius
- **minutecast**: Get minute-by-minute precipitation forecasts
- **search_city**: Search for a city by name to get its location key
- **search_geoposition**: Find a location key by latitude and longitude
- **search_ipaddress**: Find a location key by IP address
- **top_cities**: g., 50, 150).

Get a list of top cities globally or by region


## Installation & Usage

To install and use the **AccuWeather** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accuweather-alternative](https://vinkius.com/mcp/accuweather-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
