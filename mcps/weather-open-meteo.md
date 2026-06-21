# Weather (Open-Meteo) MCP Server

Get real-time weather, high-precision forecasts, air quality data, and severe weather alerts for any city worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/weather-open-meteo)

## Overview
**Category:** iot-hardware
**Tools Count:** 7

## Description
Connect to **Open-Meteo** and empower your AI agent with high-precision meteorological data through natural conversation. This server provides comprehensive weather insights for any location on Earth without requiring complex API configurations.

### What you can do

- **Current Conditions** — Retrieve real-time temperature, humidity, wind speed, and precipitation for any city
- **Precise Forecasts** — Get 7-day daily forecasts or detailed 24-hour hourly breakdowns to plan your activities
- **Air Quality** — Monitor US AQI levels and dominant pollutants (PM2.5, PM10, Ozone) with health recommendations
- **Weather Alerts** — Receive critical notifications for severe weather conditions like storms, heavy snow, or high UV levels
- **City Comparisons** — Compare weather conditions between two different cities to help with travel or logistics planning
- **Best Time Analysis** — Find the optimal window for outdoor activities based on temperature and precipitation thresholds
- **Global Coverage** — Seamlessly geocode any city name into coordinates for instant weather retrieval

### How it works

1. Subscribe to this server
2. No API Key required for non-commercial use (just click connect)
3. Start asking about the weather through Claude, Cursor, or any MCP-compatible client

No more manual browsing through weather websites. Your AI agent becomes your personal meteorologist.

### Who is this for?

- **Travelers & Planners** — find the best time for trips and compare weather between destinations
- **Outdoor Enthusiasts** — monitor air quality and identify the best windows for hiking, running, or sports
- **Logistics Teams** — check wind and precipitation conditions across different delivery routes
- **Everyday Users** — quickly check if you need an umbrella or a jacket through a simple chat command


## Available Tools
- **weather.current**: Accept natural language city names (e.g. "São Paulo", "New York", "Paris, France"). Do NOT use for forecasts — use weather.forecast for that.

Get current weather conditions for any city in the world
- **weather.forecast**: Default to 7 days if the user does not specify. Max 14 days. For today's hour-by-hour breakdown, use weather.hourly instead.

Get a multi-day weather forecast (1–14 days) for any city in the world
- **weather.hourly**: Always covers the next 24 hours from now. For multi-day overview, use weather.forecast instead.

Get an hour-by-hour weather forecast for the next 24 hours for any city
- **weather.alerts**: Alerts are computed from current conditions and the 7-day forecast. Returns an empty list if no significant conditions are detected.

Get active weather alerts and advisories for any city, derived from forecast data
- **weather.air_quality**: Always display the health_recommendation from the result. AQI scale: 0-50=Good, 51-100=Moderate, 101-150=Unhealthy for Sensitive Groups, 151-200=Unhealthy, 201-300=Very Unhealthy, 301+=Hazardous.

Get current air quality index (AQI), PM2.5, PM10, ozone, and NO2 for any city
- **weather.compare**: g. "which city has better weather?", "should I go to Lisbon or Madrid this weekend?", "compare weather in NYC, London, and Tokyo"). Accepts 2 to 5 cities. Computes a comfort score for each and highlights the best option.

Compare current weather conditions across multiple cities side by side, with comfort scores
- **weather.best_time**: This tool analyses hourly data for 72 hours and scores each 3-hour window using activity-specific criteria. Supports activities: general, hiking, beach, cycling, running, outdoor_work, photography, picnic. Always show the tip from the top-ranked window.

Find the best time windows in the next 72 hours to do an outdoor activity in any city, with a comfort score


## Installation & Usage

To install and use the **Weather (Open-Meteo)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weather-open-meteo](https://vinkius.com/mcp/weather-open-meteo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
