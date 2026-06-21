# MeteoSource MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meteosource)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor global weather — audit forecasts and places via AI.

## Description
Empower your AI agent to orchestrate your entire meteorological research and weather auditing workflow with **MeteoSource**, the comprehensive source for hyper-local weather data. By connecting the MeteoSource API to your agent, you transform complex forecast searches into a natural conversation. Your agent can instantly search for monitored places, audit daily and hourly forecasts, and retrieve timezone metadata without you ever touching a weather portal. Whether you are planning outdoor events or conducting regional climate audits, your agent acts as a real-time meteorological consultant, ensuring your data is always precise and localized.

### What you can do

- **Place Auditing** — Search for thousands of global locations and retrieve high-resolution place IDs and geographic metadata.
- **Forecast Oversight** — Audit comprehensive point forecasts, including current conditions, daily summaries, and hourly breakdowns.
- **Geographic Discovery** — Find the nearest monitored place by latitude and longitude to maintain strict organizational control over local data.
- **Temporal Intelligence** — Query timezone information for specific places to assist in time-sensitive logistics and event planning.
- **Operational Monitoring** — Check API status to ensure your meteorological research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your MeteoSource API Key
3. Start managing your weather intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners** — monitor local forecasts and retrieve weather metadata straight from your workflow.
- **Logistics Managers** — verify regional conditions and audit weather impacts on shipping patterns without manual searching.
- **Climate Researchers** — perform rapid audits of point forecasts and identify relevant monitored places through natural language.
- **Operations Leads** — automate weather data querying to orchestrate cross-functional logistics teams smoothly.


## Available Tools
- **check_api_status**: Check if the MeteoSource service is operational
- **get_point_forecast**: Get weather forecast for a specific place_id
- **get_nearest_weather_place**: Find the nearest monitored place by latitude and longitude
- **get_place_timezone**: Get timezone information for a specific place_id
- **search_weather_places**: Search for a place by name to get its place_id for forecasts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MeteoSource** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get weather forecast for 'London' using MeteoSource."

**🤖 AI Agent:**
> I've retrieved the weather for London! The current temperature is 12°C with light rain. The daily summary shows similar conditions for the next 3 days. Would you like the detailed hourly breakdown?

---

**👤 You:**
> "Search for weather station near latitude 48.8566 and longitude 2.3522."

**🤖 AI Agent:**
> I've identified the nearest place! It corresponds to Paris, France. I can retrieve the full point forecast or timezone metadata for this location if you'd like.

---

**👤 You:**
> "What is the timezone for place 'tokyo'?"

**🤖 AI Agent:**
> I've retrieved the timezone information. Tokyo is located in the 'Asia/Tokyo' timezone, currently identified as GMT+9. I can assist you with more temporal auditing if needed.


## ❓ FAQ

**Q: How do I find my MeteoSource API Key?**
Sign up for a free account at [**meteosource.com**](https://www.meteosource.com/), and you will find your API Key in your dashboard. Copy and paste it below.

**Q: Does it support location search by name?**
Yes. Use the `search_weather_places` tool providing the city or place name. Your agent will return the unique `place_id` required for forecasts.

**Q: Are hourly forecasts included?**
Yes. The `get_point_forecast` tool retrieves comprehensive weather metadata including current conditions, daily summaries, and hourly breakdowns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meteosource](https://vinkius.com/mcp/meteosource)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MeteoSource** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meteosource` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MeteoSource** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meteosource": {
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
