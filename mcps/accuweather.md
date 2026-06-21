# AccuWeather MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accuweather)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/accuweather-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/accuweather-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enterprise-grade weather intelligence — current conditions, forecasts, alarms, and activity indices via AI.

## Description
Access **AccuWeather's** superior weather forecasting — the industry standard used by enterprises worldwide for accurate, localized weather data. Connect AccuWeather to your AI agent to get current conditions, daily and hourly forecasts, severe weather alarms, and activity planning indices for any location on Earth — all through natural conversation.

### What you can do

- **Current Conditions** — Get real-time temperature, RealFeel, humidity, wind, UV index, and visibility for any city.
- **Daily Forecasts** — Retrieve 1 to 15-day forecasts with high/low temperatures, precipitation probability, and sunrise/sunset times.
- **Hourly Forecasts** — Get hour-by-hour weather for up to 120 hours (5 days) for precise planning.
- **Weather Alarms** — Monitor active severe weather alerts including hurricanes, tornadoes, floods, and heat advisories.
- **Activity Indices** — Get recommendations for outdoor activities, UV exposure, running, golf, fishing, and more.
- **Location Search** — Find any city, town, or place worldwide and get its weather.
- **Metric Units** — All data returned in Celsius, km/h, and kilometers for international use.

### How it works

1. Subscribe to this server
2. Enter your AccuWeather API Key
3. Start querying weather data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Planners** — check weather at destinations before booking trips.
- **Event Organizers** — monitor forecasts and severe weather for outdoor events.
- **Agriculture** — access extended forecasts for planting and harvest planning.
- **Emergency Management** — track severe weather alarms for public safety.


## Available Tools
- **get_weather_alarms**: Includes severe weather alerts such as hurricanes, tornadoes, flood warnings, heat advisories, and winter storm warnings. Each alarm includes severity level, description, start and end times, and source. Essential for safety planning, emergency preparedness, and travel decisions. Returns empty if no active alarms.

Get active weather alarms and warnings for a location
- **get_current_conditions**: Returns temperature (metric), weather text (e.g. "Partly sunny"), RealFeel temperature, humidity, wind speed and direction, UV index, visibility, cloud cover, and precipitation. Essential for instant weather checks. Use get_location_by_key first to find the correct location key.

Get current weather conditions for a location
- **get_current_conditions_metric**: Returns temperature in Celsius, wind in km/h, visibility in kilometers. Includes RealFeel temperature, humidity, UV index, wind gusts, and precipitation data. Use for international audiences or scientific analysis.

Get current weather conditions with detailed metric values
- **get_daily_forecast**: Each day includes high and low temperatures, weather conditions, precipitation probability, wind speed, UV index, sunrise/sunset times, and air quality information. Returns data in metric units (Celsius, km/h). Essential for trip planning, event scheduling, and agricultural decisions. Use 5 days for standard weekly forecasts.

Get daily weather forecast for a location
- **get_extended_forecast**: While forecasts beyond 7-10 days have lower accuracy, this is useful for event planning, travel preparation, and agricultural scheduling. Each day includes high/low temperatures, precipitation probability, and general conditions. Use for planning events 2 weeks in advance.

Get 15-day extended weather forecast
- **get_hourly_forecast**: Each hour includes temperature, weather icon, precipitation probability, wind speed and direction, and cloud cover. Essential for detailed planning — knowing exactly when rain will start, when temperatures peak, or when conditions are safe for outdoor activities. Returns data in metric units. Use 24 hours for tomorrow planning.

Get hourly weather forecast for a location
- **get_index_groups**: This helps you understand what types of indices are available (outdoor activities, health, home & garden, etc.) before querying specific indices for a location. Use this to discover what activity planning indices are supported.

Get available index groups and categories
- **get_weather_indices**: Includes indices for outdoor activity suitability, flight delay probability, UV exposure, running, hiking, golf, fishing, lawn mowing, composting, and more. Each index includes a numeric value, category (e.g. "Excellent", "Poor", "Good"), and descriptive text. Essential for activity planning, health advisories, and lifestyle decisions.

Get weather indices (outdoor activity, flight, UV, etc.) for a location
- **get_location_by_key**: Returns the city name, country, region, timezone, coordinates, elevation, and administrative area. Use this to verify you have the correct location before making weather queries.

Get detailed information about a location by its AccuWeather key
- **search_location**: The location key is required for other weather queries. Returns matching locations with their keys, country, region, and coordinates. Use this as the first step before any weather query. For example, search for "New York" to find the correct location key for New York City. Supports partial matching and returns multiple results.

Search for a location by name to get its AccuWeather location key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AccuWeather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather like in Tokyo right now?"

**🤖 AI Agent:**
> Current conditions in Tokyo: 22°C with partly cloudy skies. RealFeel is 24°C, humidity at 65%, and wind from the southeast at 8 km/h. UV index is moderate at 5. No precipitation expected.

---

**👤 You:**
> "Give me the 5-day forecast for Paris, France."

**🤖 AI Agent:**
> Here's the 5-day forecast for Paris: Today 24°C/14°C with sunshine, Friday 21°C/13°C with possible afternoon showers, Saturday 18°C/11°C cloudy, Sunday 17°C/10°C with rain, Monday 20°C/12°C clearing up. Sunrise at 6:42 AM, sunset at 8:58 PM.

---

**👤 You:**
> "Are there any severe weather alerts for Miami right now?"

**🤖 AI Agent:**
> There is currently a Heat Advisory in effect for Miami-Dade County until 7 PM EDT. Heat index values up to 41°C are expected. Take precautions for heat-related illness. No other active alerts for this area.


## Installation & Usage

To install and use the **AccuWeather** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accuweather](https://vinkius.com/mcp/accuweather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
