# AerisWeather MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aerisweather)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access hyper-local weather data, forecasts, and alerts via AerisWeather — query observations, conditions, and geographical data directly from any AI agent.

## Description
Connect your **AerisWeather** account to any AI agent and access professional-grade weather intelligence through natural conversation.

### What you can do

- **Observations & Forecasts** — Fetch real-time METAR/PWS data and up to 15-day forecasts for any global location using `get_observations` and `get_forecasts`.
- **Global Conditions** — Get interpolated current, forecast, and historical weather conditions with minute-by-minute precipitation via `get_conditions`.
- **Weather Alerts** — Monitor active warnings, watches, and advisories from official sources like NWS and MeteoAlarm using `get_alerts`.
- **Geographical Data** — Retrieve detailed place information including timezones, population, and coordinates for cities or airports with `get_places`.
- **Batch Processing** — Efficiently query multiple endpoints in a single request to optimize agent performance using `get_batch`.

### How it works

1. Subscribe to this server
2. Enter your AerisWeather Client ID and Client Secret
3. Start querying weather data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Integrate weather context into applications or automation scripts directly from the IDE.
- **Logistics & Operations** — Monitor weather alerts and conditions for fleet management or event planning.
- **Data Analysts** — Access historical and real-time weather datasets for environmental research or business intelligence.


## Available Tools
- **get_alerts**: Get active weather warnings, watches, and advisories
- **get_batch**: Action is usually a location ID. Provide a comma-separated list of requests (e.g., /observations,/forecasts,/alerts). Max 31 requests.

Query multiple endpoints in a single request for efficiency
- **get_conditions**: Supports minutely precipitation forecasts (filter=minutelyprecip). Range: 2004 to +15 days.

Get interpolated global current, forecast, and historical conditions
- **get_forecasts**: Get weather forecasts
- **get_observations**: Action can be an ID (e.g., minneapolis,mn), closest, search, or within.

Get current weather observations
- **get_places**: Get geographical data for cities, stations, and airports


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AerisWeather** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current weather in London?"

**🤖 AI Agent:**
> I've retrieved the current conditions for London. It's currently 15°C with light rain and a humidity of 78%. Would you like the forecast for the rest of the day?

---

**👤 You:**
> "Show me the 7-day forecast for New York."

**🤖 AI Agent:**
> Fetching the 7-day forecast for New York... I see a mix of sun and clouds for the next few days, with temperatures peaking at 22°C on Wednesday. Should I check for any precipitation alerts?

---

**👤 You:**
> "Are there any active weather alerts for Miami?"

**🤖 AI Agent:**
> Checking for active alerts in Miami... There is currently a 'Flood Watch' in effect until 8:00 PM. Would you like to see the full details of the advisory?


## ❓ FAQ

**Q: Can I get minute-by-minute precipitation forecasts?**
Yes! Use the `get_conditions` tool with the `filter` parameter set to `minutelyprecip`. This provides high-resolution precipitation data for the immediate future.

**Q: How do I check for active weather warnings in a specific area?**
Use the `get_alerts` tool and provide the location in the `p` parameter. It will return active watches, warnings, and advisories from official meteorological agencies.

**Q: Is it possible to search for cities or airports by name?**
Yes! Use the `get_places` tool with the `action` set to `search` and your query. It returns geographical metadata, timezones, and coordinates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aerisweather](https://vinkius.com/mcp/aerisweather)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AerisWeather** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aerisweather` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AerisWeather** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aerisweather": {
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
