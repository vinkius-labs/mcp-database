# Weather (Open-Meteo) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weather-open-meteo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Get real-time weather, high-precision forecasts, air quality data, and severe weather alerts for any city worldwide.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weather (Open-Meteo)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the weather like in Tokyo right now?"

**🤖 AI Agent:**
> In Tokyo, Japan, it's currently 18°C with partly cloudy skies (⛅). The humidity is 65% and there is a light breeze from the South at 12 km/h. It feels like 17°C.

---

**👤 You:**
> "Give me the 7-day forecast for London."

**🤖 AI Agent:**
> Here is the 7-day forecast for London: Tomorrow will be rainy with a high of 14°C. Wednesday looks clear and sunny (☀️) at 16°C. The rest of the week will be mostly cloudy with temperatures between 12°C and 15°C. Would you like the hourly details for any specific day?

---

**👤 You:**
> "Compare the weather between New York and Miami."

**🤖 AI Agent:**
> Comparing conditions: New York is currently 8°C and overcast (☁️), while Miami is much warmer at 26°C with clear skies (☀️). New York is experiencing light rain, whereas Miami is dry. It's significantly warmer in Miami right now.


## ❓ FAQ

**Q: Do I need an API key to use this weather server?**
No. This server uses the Open-Meteo API, which is free and open-source for non-commercial use. You can start using it immediately without any manual configuration or signup processes.

**Q: Can I check the air quality for my city?**
Yes. The `weather.air_quality` tool provides the current US AQI level, concentrations of PM2.5, PM10, Ozone, and health recommendations based on the current conditions.

**Q: How can I find the best time for a run or a hike?**
Use the `weather.best_time` tool. You can specify your preferred temperature range and whether you want to avoid rain. Your agent will analyze the forecast and suggest the optimal time windows for your activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weather-open-meteo](https://vinkius.com/mcp/weather-open-meteo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weather (Open-Meteo)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weather-open-meteo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weather (Open-Meteo)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weather-open-meteo": {
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
