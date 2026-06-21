# SPTrans Olho Vivo MCP Server

Access real-time public transit data for São Paulo — track bus positions, check arrival forecasts, and locate stops across the city.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sptrans-olho-vivo)

## Overview
**Category:** data-analytics
**Tools Count:** 13

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


## Installation & Usage

To install and use the **SPTrans Olho Vivo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sptrans-olho-vivo](https://vinkius.com/mcp/sptrans-olho-vivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
