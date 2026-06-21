# Tomorrow.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomorrowio-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access hyperlocal weather intelligence — real-time conditions, forecasts, historical archives, severe alerts and route weather from the Tomorrow.io API.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tomorrow.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather like in Tokyo right now?"

**🤖 AI Agent:**
> Currently in Tokyo: 🌡️ 18.5°C, 💧 62% humidity, 💨 12 km/h NW wind, clear skies with 0% precipitation probability. UV index is 3 (moderate). Visibility is excellent at 16 km.

---

**👤 You:**
> "Give me an hourly forecast for São Paulo for the next 12 hours."

**🤖 AI Agent:**
> Hourly forecast for São Paulo: 14:00 — 27°C, 45% humidity, 8% rain chance | 15:00 — 28°C, 42%, 5% | 16:00 — 26°C, 55%, 25% | 17:00 — 24°C, 68%, 60% — thunderstorm likely | 18:00 — 22°C, 78%, 85% — heavy rain expected. I'd recommend carrying an umbrella after 4 PM.

---

**👤 You:**
> "What was the weather like in London on January 15, 2025?"

**🤖 AI Agent:**
> Historical weather for London on January 15, 2025: High 7.2°C, Low 2.1°C, 89% humidity, 22 km/h SW wind, 4.8mm rainfall recorded, overcast skies throughout the day. Visibility was reduced to 8km due to light drizzle in the morning.


## ❓ FAQ

**Q: What weather data points can I retrieve with this integration?**
You can retrieve temperature, humidity, wind speed/direction/gusts, precipitation intensity/probability, UV index, visibility, cloud cover, dew point, pressure, snow accumulation, air quality index and more. Use the `get_timeline` tool to specify exactly which fields you need.

**Q: How far back can I access historical weather data?**
The `get_historical_weather` tool can access archived weather data going back up to 20 years. For the most recent 24 hours, use `get_recent_history` which provides higher-resolution data. Historical data availability depends on your Tomorrow.io plan tier.

**Q: Can I get weather conditions along a driving route?**
Yes! The `get_route_weather` tool accepts a series of waypoints (each with latitude, longitude and expected arrival time) and returns weather forecasts for each segment. Perfect for logistics planning, road trips and delivery optimization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomorrowio-alternative](https://vinkius.com/mcp/tomorrowio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tomorrow.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tomorrowio-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tomorrow.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tomorrowio-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
