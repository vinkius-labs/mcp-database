# Tomorrow.io MCP Server

Access hyperlocal weather intelligence — real-time conditions, forecasts, historical archives, severe alerts and route weather from the Tomorrow.io API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tomorrowio-alternative)

## Overview
**Category:** iot-hardware
**Tools Count:** 10

## Description
Connect your **Tomorrow.io** account to any AI agent and unlock enterprise-grade weather intelligence through natural conversation.

### What you can do

- **Real-time Conditions** — Get current temperature, humidity, wind, precipitation, UV index, visibility and air quality for any location worldwide
- **Multi-Resolution Forecasts** — Access minute-by-minute, hourly (120h) and daily (14-day) weather forecasts with precipitation probability, wind and pressure
- **Historical Weather Archive** — Query up to 20 years of archived weather data for climate analysis, insurance claims and agricultural research
- **Recent History** — Retrieve actual observed conditions from the last 24 hours to verify weather events
- **Custom Timelines** — Build precise queries with specific fields, timesteps and date ranges for dashboards and analytics
- **Severe Weather Alerts** — Monitor active weather events, storm warnings, heat advisories and meteorological hazards
- **Route Weather** — Plan logistics and road trips by getting weather conditions along any multi-waypoint route

### How it works

1. Subscribe to this server
2. Sign up at [Tomorrow.io](https://app.tomorrow.io/) and generate your free API key
3. Start querying weather data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate weather data into applications, dashboards and automated workflows
- **Operations & Logistics** — plan deliveries, routes and outdoor events with precise forecasts
- **Researchers & Analysts** — access 20+ years of historical weather data for climate studies
- **Agriculture & Insurance** — verify weather conditions for crop planning and claims processing


## Available Tools
- **get_daily_forecast**: Perfect for weekly planning and travel preparation.

Get daily weather forecast for a location
- **get_weather_events**: Returns severe weather warnings, storm alerts, heat advisories and other meteorological events that may impact the area.

Get active weather events and alerts for a location
- **get_forecast**: Returns temperature, precipitation probability, wind, humidity and more for up to 14 days ahead depending on plan. Default includes all available timesteps.

Get weather forecast for a location
- **get_historical_weather**: Specify a date range and the weather fields you need. Returns daily or hourly observed data. Useful for climate analysis, insurance claims, and research.

Get historical weather data for a date range
- **get_hourly_forecast**: Returns temperature, precipitation, wind, humidity and pressure for each hour. Ideal for planning activities in the next few days.

Get hourly weather forecast for a location
- **list_locations**: io developer account. Useful for managing frequently monitored areas and checking which locations have active insights configured.

List saved locations in your Tomorrow.io account
- **get_realtime_weather**: Accepts city names, coordinates (lat,lng), or US zip codes.

Get current real-time weather conditions for a location
- **get_recent_history**: Returns actual observed conditions including temperature, precipitation, wind and humidity. Useful for verifying recent weather events.

Get weather data from the last 24 hours
- **get_route_weather**: Perfect for logistics, road trips and delivery planning. Each waypoint needs latitude, longitude and time in ISO 8601 format.

Get weather along a travel route
- **get_timeline**: Specify exactly which data points you need (e.g. temperature, humidity, windSpeed, precipitationProbability) and at what interval. Ideal for custom analytics and dashboards.

Get custom weather timeline with specific fields and timesteps


## Installation & Usage

To install and use the **Tomorrow.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomorrowio-alternative](https://vinkius.com/mcp/tomorrowio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
