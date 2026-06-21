# OpenWeatherMap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openweathermap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openweathermap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openweathermap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time weather data, 5-day forecasts, air quality metrics, and geocoding services globally via OpenWeatherMap.

## Description
Connect **OpenWeatherMap** to your AI agent to get instant access to global meteorological data. Whether you're planning travel, monitoring environmental conditions, or building weather-aware automations, this server provides the precise data you need.

### What you can do

- **Current Conditions** — Get live temperature, humidity, wind speed, and weather descriptions for any city or coordinate via `get_current_weather`.
- **Extended Forecasts** — Access 5-day/3-hour forecasts with `get_forecast` or use the One Call 3.0 API for 48-hour hourly and 8-day daily projections via `get_onecall`.
- **Air Quality Monitoring** — Retrieve real-time pollution data including PM2.5, PM10, CO, and Ozone levels using `get_air_pollution`.
- **Geocoding Services** — Seamlessly convert city names to coordinates with `direct_geocoding` and vice versa with `reverse_geocoding` to power location-based queries.

### How it works

1. Subscribe to this server
2. Enter your OpenWeatherMap API Key
3. Ask about weather or air quality in any location from Claude, Cursor, or any MCP client

### Who is this for?

- **Travelers & Logistics** — Check conditions at destinations or along routes to optimize schedules.
- **Developers** — Integrate weather context into apps and workflows without leaving your code editor.
- **Environmental Researchers** — Monitor air quality and weather patterns across different coordinates instantly.


## Available Tools
- **get_air_pollution**: 5, PM10, and NH3.

Get current air pollution data
- **get_current_weather**: Get current weather data
- **direct_geocoding**: Convert city names or zip codes into coordinates
- **get_forecast**: Get 5 Day / 3 Hour Forecast
- **get_onecall**: Get One Call API 3.0 weather data
- **reverse_geocoding**: Convert coordinates into city names


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenWeatherMap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current weather in London?"

**🤖 AI Agent:**
> Using `get_current_weather` for London... It's currently 15°C with light rain and 82% humidity.

---

**👤 You:**
> "Give me the 5-day forecast for Tokyo."

**🤖 AI Agent:**
> Fetching the 5-day forecast via `get_forecast`... Tokyo will see mostly clear skies for the next 3 days, with temperatures ranging from 18°C to 24°C.

---

**👤 You:**
> "Check the air pollution levels at latitude 40.71 and longitude -74.00."

**🤖 AI Agent:**
> Running `get_air_pollution` for those coordinates... The Air Quality Index is 2 (Fair). PM2.5 is at 12.5 μg/m³ and CO is at 320.4 μg/m³.


## Installation & Usage

To install and use the **OpenWeatherMap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openweathermap](https://vinkius.com/mcp/openweathermap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
