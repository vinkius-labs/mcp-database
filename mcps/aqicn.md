# AQICN MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aqicn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time Air Quality Index (AQI) data, pollutant levels, and weather conditions from over 30,000 stations worldwide.

## Description
Connect to the **AQICN (World Air Quality Index)** project and bring real-time environmental intelligence to your AI agent. Monitor pollution levels, track specific pollutants like PM2.5 or O3, and get localized weather data through natural language commands.

### What you can do

- **City-Level Feeds** — Get instant AQI reports for major cities globally using the `get_city_feed` tool.
- **Station-Specific Data** — Query precise monitoring stations using unique IDs with `get_station_feed` for hyper-local accuracy.
- **IP-Based Location** — Automatically detect the nearest station based on your current connection using `get_ip_feed`.
- **Global Search** — Find monitoring stations by name or keyword in any region with `search_stations`.
- **Map Bounding Boxes** — Retrieve all active stations within specific geographic coordinates using `get_map_bounds`.

### How it works

1. Subscribe to this server
2. Enter your AQICN API Token
3. Start monitoring air quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health-Conscious Users** — Check if it's safe for outdoor activities based on real-time PM2.5 levels.
- **Environmental Researchers** — Gather data across multiple stations for analysis without manual scraping.
- **Travelers & Expats** — Verify the air quality of your destination before you arrive or monitor your current city.


## Available Tools (5)
- **get_city_feed**: Get real-time Air Quality Index for a specific city
- **get_ip_feed**: Get real-time Air Quality Index based on IP location
- **get_map_bounds**: Get all stations within a specific map bounding box
- **search_stations**: Search for air quality monitoring stations
- **get_station_feed**: Get real-time Air Quality Index for a specific station by UID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AQICN** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the current air quality in London?"

**🤖 AI Agent:**
> I've checked the feed for London. The current AQI is 42 (Good), with PM2.5 as the primary pollutant. The temperature is 12°C with 78% humidity.

---

**👤 You:**
> "Search for air quality monitoring stations in Beijing."

**🤖 AI Agent:**
> I found several stations in Beijing. The main station (UID 1451) reports an AQI of 156 (Unhealthy). Other nearby stations include Dongsi and Temple of Heaven.

---

**👤 You:**
> "Show me all air quality stations within these coordinates: 39.37,116.09,40.23,116.78."

**🤖 AI Agent:**
> Scanning the area... I've identified 8 active stations within those bounds. AQI levels range from 140 to 165 across the grid. Would you like the specific details for the station with the highest pollution?


## ❓ FAQ

**Q: How can I find the AQI for a specific station ID?**
Use the `get_station_feed` tool and provide the unique station UID. The agent will return real-time AQI, pollutant breakdowns, and local weather conditions for that exact location.

**Q: Can I see all stations in a specific geographic area?**
Yes! Use the `get_map_bounds` tool by providing the latitude and longitude coordinates for the north, west, south, and east boundaries of your target area.

**Q: Is it possible to search for stations by name?**
Absolutely. Use the `search_stations` tool with a keyword like 'Bangalore' or 'London' to get a list of all matching monitoring stations and their current AQI levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aqicn](https://vinkius.com/mcp/aqicn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AQICN** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aqicn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AQICN** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aqicn": {
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
