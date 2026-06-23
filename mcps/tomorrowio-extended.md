# Tomorrow.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tomorrowio-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Hyper-local weather intelligence platform — get realtime, forecast, and air quality data via AI.

## Description
Equip your AI agent with the world's most accurate weather intelligence via **Tomorrow.io**. This integration provides your agent with real-time access to hyper-local weather conditions, minute-by-minute forecasts, and deep atmospheric data. Your agent can instantly check the current temperature, audit historical trends, and monitor air quality levels without you ever touching a weather app. Whether you are planning logistics or managing outdoor operations, your agent acts as a dedicated meteorologist, ensuring your decisions are always guided by precise environmental data.

### What you can do

- **Realtime Conditions** — Access current weather data including temperature, humidity, and wind speed for any location.
- **Forecast Auditing** — Retrieve detailed weather forecasts with customizable timesteps (1m, 1h, 1d).
- **Historical Trends** — Fetch recent weather history to analyze environmental patterns over the last 24 hours.
- **Air Quality Monitoring** — Monitor pollution levels and air quality indices to ensure safe environmental conditions.
- **Weather Alerts** — Stay updated on active weather warnings and alerts issued for specific geographic areas.

### How it works

1. Subscribe to this server
2. Enter your Tomorrow.io API Key
3. Start managing your weather intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Supply Chain Managers** — optimize routes and operations based on precise weather forecasts.
- **Event Organizers** — monitor environmental conditions to ensure the safety and success of outdoor gatherings.
- **Agricultural Professionals** — track hyper-local weather patterns to optimize irrigation and harvesting schedules.
- **Smart Home Enthusiasts** — automate home systems based on realtime temperature and air quality data.
- **Travelers & Outdoor Enthusiasts** — get minute-by-minute weather updates for their specific adventure locations.


## Available Tools (5)
- **get_air_quality**: Get air quality data
- **list_weather_alerts**: List weather alerts
- **get_weather_forecast**: Get weather forecast
- **get_recent_history**: Get recent weather history
- **get_realtime_weather**: Get realtime weather data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tomorrow.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current weather in London?"

**🤖 AI Agent:**
> Checking realtime data for London... It's currently 15°C with clear skies and a light breeze. Humidity is at 65%.

---

**👤 You:**
> "Give me the hourly forecast for San Francisco."

**🤖 AI Agent:**
> Retrieving the hourly forecast for San Francisco... You can expect temperatures to range between 12°C and 18°C today, with some fog rolling in around 6 PM.

---

**👤 You:**
> "How is the air quality in Beijing today?"

**🤖 AI Agent:**
> Fetching air quality data for Beijing... The AQI is currently 120 (Unhealthy for Sensitive Groups), primarily due to PM2.5 levels. I recommend minimizing outdoor activities if you are sensitive.


## ❓ FAQ

**Q: Can I get weather updates for a specific set of coordinates?**
Yes! You can provide coordinates (latitude, longitude) in the `location` parameter for any tool to get hyper-local data for that exact point.

**Q: What timesteps are supported for weather forecasts?**
Tomorrow.io supports `1m` (minute-by-minute), `1h` (hourly), and `1d` (daily) timesteps. Specify your preference in the `timesteps` parameter of the `get_weather_forecast` tool.

**Q: Does the air quality tool provide specific pollutant levels?**
Yes, the `get_air_quality` tool retrieves data for various pollutants including PM2.5, PM10, O3, NO2, and CO, along with the overall Air Quality Index (AQI).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomorrowio-extended](https://vinkius.com/mcp/tomorrowio-extended)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `tomorrowio-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tomorrow.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tomorrowio-extended": {
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
