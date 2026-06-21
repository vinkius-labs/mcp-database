# SPTrans Olho Vivo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sptrans-olho-vivo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sptrans-olho-vivo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sptrans-olho-vivo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time public transit data for São Paulo — track bus positions, check arrival forecasts, and locate stops across the city.

## Description
Connect to the **SPTrans Olho Vivo** API to bring real-time urban mobility intelligence to your AI agent. Monitor the entire São Paulo bus fleet and provide precise transit information through natural conversation.

### What you can do

- **Line & Stop Discovery** — Search for bus lines by name or number and find specific stops by address or corridor.
- **Real-time GPS Tracking** — Fetch the exact coordinates of active buses on any given line or across the entire city fleet.
- **Arrival Forecasts** — Get accurate predictions for when the next bus will arrive at a specific stop or for all stops along a route.
- **Corridor & Company Info** — List intelligent bus corridors and operating companies to understand the city's transit infrastructure.
- **Garage Status** — Monitor vehicles currently in the garage for specific companies and lines.

### How it works

1. Subscribe to this server
2. Enter your SPTrans Olho Vivo API Token
3. Start querying São Paulo's transit system from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Commuters & Residents** — Get instant updates on bus arrivals and locations without switching between multiple transit apps.
- **Urban Planners & Researchers** — Analyze real-time fleet distribution and corridor efficiency directly through AI-driven data extraction.
- **Developers** — Integrate São Paulo's transit data into workflows or tools using simple natural language commands.


## Available Tools
- **get_forecast_by_line**: Get arrival forecast for all stops on a specific line
- **get_forecast_by_stop**: Get arrival forecast for all lines arriving at a specific stop
- **get_forecast**: Get arrival forecast for a specific stop and line
- **get_positions_by_line**: Get real-time GPS positions for buses on a specific line
- **get_positions_in_garage**: Get real-time GPS positions for buses currently in the garage
- **get_all_positions**: Get real-time GPS positions for all active buses
- **list_companies**: List bus operating companies by area
- **list_corridors**: List all intelligent bus corridors in São Paulo
- **search_lines_by_direction**: Search for bus lines filtered by direction
- **search_lines**: Search for bus lines by number or name
- **search_stops_by_corridor**: Get all stops in a specific intelligent corridor
- **search_stops_by_line**: Get all stops for a specific bus line
- **search_stops**: Search for bus stops by name or address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SPTrans Olho Vivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for bus lines related to 'Lapa'."

**🤖 AI Agent:**
> I found several lines for 'Lapa', including line 8000-10 (Terminal Lapa) with code 33657. Would you like to see the current bus positions for this line?

---

**👤 You:**
> "What are the arrival forecasts for stop code 650005666?"

**🤖 AI Agent:**
> For stop 650005666, the next bus on line 8000-10 is expected in 5 minutes. There is also a bus for line 8615-10 arriving in 12 minutes.

---

**👤 You:**
> "Show me the real-time positions of buses on line 33657."

**🤖 AI Agent:**
> There are currently 4 buses active on line 33657. Two are near Terminal Lapa, one is on Rua Clélia, and one is approaching the city center.


## Installation & Usage

To install and use the **SPTrans Olho Vivo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sptrans-olho-vivo](https://vinkius.com/mcp/sptrans-olho-vivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
