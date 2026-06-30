# QWeather / 和风天气 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qweather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Leading professional weather data service in China — retrieve forecasts, air quality, and life indices via AI.

## Description
Empower your AI agent to orchestrate your daily planning and environmental monitoring with **QWeather** (和风天气), the premier commercial weather platform in China. By connecting QWeather to your agent, you transform complex meteorological data and location-based environmental searches into a natural conversation. Your agent can instantly retrieve real-time weather, 15-day forecasts, air quality indices, severe weather warnings, and astronomical data without you ever needing to navigate a technical dashboard. Whether you are planning outdoor operations or auditing air quality across different regions, your agent acts as a real-time environmental consultant, providing accurate and fast results from a single, unified source.

### What you can do

- **Weather Orchestration** — Retrieve current weather and detailed forecasts (up to 15 days) for any location worldwide.
- **Air Quality Auditing** — Monitor real-time AQI, PM2.5, and PM10 levels to ensure safe operating conditions.
- **Life Index Insights** — Access specialized indices for UV radiation, clothing recommendations, and car washing suitability.
- **Warning Monitoring** — Audit active severe weather warnings to maintain safety and organizational continuity.
- **Geographic Discovery** — Search for location IDs and coordinates using keywords to refine your regional tracking.

### How it works

1. Subscribe to this server
2. Enter your QWeather API Key and specify your plan (dev/free/standard/premium)
3. Start querying environmental data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor weather conditions for logistics and outdoor events through natural language queries.
- **HSE Professionals** — audit air quality and weather warnings directly from your AI-powered workspace.
- **Developers** — integrate professional meteorological data into your AI-driven daily routines.
- **QWeather Power Users** — integrate your existing environmental workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_weather_24h**: Get 24-hour weather forecast
- **get_air_now**: 5, etc.).

Get current air quality
- **get_indices**: Get daily life indices
- **get_moon_astronomy**: Get moonrise and moonset times
- **get_sun_astronomy**: Get sunrise and sunset times
- **get_warning**: Get weather warnings
- **get_weather_3d**: Get 3-day weather forecast
- **get_weather_7d**: Get 7-day weather forecast
- **get_weather_now**: Get current weather
- **lookup_location**: Search for location ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QWeather / 和风天气** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current weather in Beijing (101010100)?"

**🤖 AI Agent:**
> The current weather in Beijing is clear with a temperature of 22°C. The humidity is 45% and the air quality is excellent (AQI: 35). Would you like to see the forecast for the next 3 days?

---

**👤 You:**
> "Check the air quality for Shanghai today."

**🤖 AI Agent:**
> I've retrieved the air quality for Shanghai. The current AQI is 75 (Moderate). PM2.5 levels are at 25 μg/m³. Outdoor activities are generally safe, but sensitive individuals should monitor the situation.

---

**👤 You:**
> "Find the location ID for 'Hangzhou'."

**🤖 AI Agent:**
> I've found the location ID for Hangzhou. The ID is `101210101`. It is located in Zhejiang, China. I can now use this ID to retrieve detailed weather or air quality data for you.


## ❓ FAQ

**Q: How do I find my QWeather API Key?**
Log in to the [QWeather Developer Console](https://dev.qweather.com/), create a project, and your API Key will be displayed in the project settings. Ensure you select the correct key type (Web API).

**Q: What is the difference between dev and commercial plans?**
The 'dev' plan uses `devapi.qweather.com` and has limited data frequency and locations. Commercial plans (standard/premium) use `api.qweather.com` and provide higher resolution data and broader global coverage. Set your `qweather_plan` in the credentials to use the correct endpoint.

**Q: Can I query weather by coordinates?**
Yes! You can pass coordinates in the format `longitude,latitude` (e.g., '116.41,39.92') to any tool that accepts a `location` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qweather](https://vinkius.com/mcp/qweather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QWeather / 和风天气** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qweather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QWeather / 和风天气** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qweather": {
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
