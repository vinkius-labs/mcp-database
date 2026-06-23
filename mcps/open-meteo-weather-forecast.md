# Open-Meteo Weather Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-meteo-weather-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Give your AI agent live weather intelligence: 16-day forecasts, current conditions, and hourly breakdowns for any GPS coordinate on Earth — zero API keys required.

## Description
Connect your AI agent to the world's most comprehensive **open weather API** — no API key, no registration, no rate-limit headaches.

### What you can do
- **16-Day Forecast** — Hourly and daily predictions with temperature, precipitation probability, wind, humidity, UV index, and weather codes
- **Current Conditions** — Real-time snapshot including apparent temperature, cloud cover, wind gusts, and precipitation status
- **Hourly Granularity** — Dewpoint, visibility, snow depth, solar radiation, evapotranspiration, and CAPE convective index
- **Daily Summaries** — Max/min temperature, sunrise/sunset times, sunshine duration, and dominant wind direction

### How it works
1. Subscribe to this server — it's free and instant.
2. No API keys needed — Open-Meteo is open data.
3. Ask your AI about any location's weather.

### Who is this for?
Logistics planners, agriculture professionals, event organizers, travel apps, and anyone building weather-aware AI agents.


## Available Tools (4)
- **get_weather_forecast**: Provide latitude and longitude coordinates.

Get weather forecast for any location (up to 16 days)
- **get_current_weather**: Provide latitude and longitude.

Get current weather conditions for any location
- **get_hourly_details**: Get detailed hourly weather data
- **get_daily_summary**: Get daily weather summary with sunrise/sunset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open-Meteo Weather Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather forecast for Tokyo this week?"

**🤖 AI Agent:**
> 🌦️ **Tokyo 7-Day Forecast**

Today: 22°C, partly cloudy, 10% rain chance
Tomorrow: 19°C, rain expected (85%), 12mm precipitation
Wednesday: 24°C, sunny, UV index 7 (high)

Wind speeds remain moderate at 15-20 km/h from the southeast.

---

**👤 You:**
> "What are the current weather conditions in New York?"

**🤖 AI Agent:**
> 🌡️ **New York — Current Conditions**

- Temperature: 18°C (feels like 16°C)
- Humidity: 62%
- Wind: 22 km/h NW, gusts up to 35 km/h
- Cloud cover: 45%
- Precipitation: None currently

---

**👤 You:**
> "Will it snow in Munich in the next 10 days?"

**🤖 AI Agent:**
> ❄️ **Munich 10-Day Snow Analysis**

Snowfall detected on days 4-5:
- Day 4: 3.2mm snow, -2°C
- Day 5: 1.8mm snow, -1°C
- Snow depth expected to reach 5cm

All other days remain above freezing with no snow expected.


## ❓ FAQ

**Q: Do I need an API key?**
No! Open-Meteo is completely free and open. This server works instantly with zero configuration — just subscribe and start asking about the weather.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-meteo-weather-forecast](https://vinkius.com/mcp/open-meteo-weather-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open-Meteo Weather Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-meteo-weather-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open-Meteo Weather Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-meteo-weather-forecast": {
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
