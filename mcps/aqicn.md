# AQICN MCP Server

Access real-time Air Quality Index (AQI) data, pollutant levels, and weather conditions from over 30,000 stations worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aqicn)

## Overview
**Category:** data-analytics
**Tools Count:** 5

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


## Available Tools
- **get_city_feed**: Get real-time Air Quality Index for a specific city
- **get_ip_feed**: Get real-time Air Quality Index based on IP location
- **get_map_bounds**: Get all stations within a specific map bounding box
- **search_stations**: Search for air quality monitoring stations
- **get_station_feed**: Get real-time Air Quality Index for a specific station by UID


## Installation & Usage

To install and use the **AQICN** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aqicn](https://vinkius.com/mcp/aqicn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
