# AccuWeather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accuweather-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time weather data, detailed forecasts, and location-based climate insights directly from your AI agent using AccuWeather's global network.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AccuWeather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the city 'London' and tell me the current weather conditions."

**🤖 AI Agent:**
> I've found London (Location Key: 328328). The current conditions are: Overcast, 12°C with a humidity of 82%. Would you like the hourly forecast as well?

---

**👤 You:**
> "What is the 5-day forecast for location key 349727?"

**🤖 AI Agent:**
> Fetching the 5-day forecast for New York (349727)... Expect sunny intervals on Monday (High 22°C), followed by light rain on Tuesday and Wednesday. Thursday and Friday will be clear and cool.

---

**👤 You:**
> "Find the location key for coordinates 40.7128, -74.0060."

**🤖 AI Agent:**
> The coordinates 40.7128, -74.0060 correspond to New York, NY. The Location Key is 349727. I can now fetch forecasts or current conditions for this area.


## ❓ FAQ

**Q: How do I find the weather for a specific city if I don't have its location key?**
First, use the `search_city` tool with the city name. It will return a 'Location Key'. You can then use that key with tools like `current_conditions` or `daily_forecast` to get the weather data.

**Q: Can I get weather forecasts for multiple days at once?**
Yes! Use the `daily_forecast` tool and specify the `period` parameter (e.g., '5day' or '10day'). This will provide a structured forecast for the requested duration.

**Q: Is it possible to search for weather using just GPS coordinates?**
Absolutely. Use the `search_geoposition` tool and provide the latitude and longitude (e.g., '40.7128,-74.0060'). The agent will find the corresponding location key for you.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accuweather-alternative](https://vinkius.com/mcp/accuweather-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AccuWeather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `accuweather-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AccuWeather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accuweather-alternative": {
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
