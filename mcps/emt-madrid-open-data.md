# EMT Madrid (Open Data) MCP Server

Access real-time Madrid public transport data: bus arrivals, BiciMAD bike status, and route planning via EMT Open Data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/emt-madrid-open-data)

## Overview
**Category:** government-public-data
**Tools Count:** 4

## Description
Connect to the **EMT Madrid Open Data** platform to bring Madrid's mobility network into your AI agent. This server provides direct access to official transport data for the city of Madrid.

### What you can do

- **Real-time Bus Arrivals** — Use `get_bus_arrivals` to see exactly when the next bus is reaching a specific stop using its unique ID.
- **BiciMAD Integration** — Use `list_bicimad_stations` to check bike availability and empty docks across the city's electric bike-sharing system.
- **Route Planning** — Use `plan_bus_route` to find the best way to navigate the city using the EMT bus network from any starting stop.
- **Official Data** — Access the same data used by official apps to ensure accuracy in your mobility workflows.

### How it works

1. Subscribe to this server
2. Provide your EMT MobilityLabs API Key
3. Start asking about Madrid's transport from Claude, Cursor, or any MCP client.

### Who is this for?

- **Commuters** — Get quick updates on your daily route without opening multiple apps.
- **Developers** — Integrate Madrid's transport data into custom mobility tools or dashboards.
- **Travelers** — Navigate Madrid like a local with real-time transit information.


## Available Tools
- **list_bicimad_stations**: Get status of all BiciMAD stations
- **get_bus_arrivals**: Get real-time bus arrival times for a stop
- **login**: Login to EMT MobilityLabs to get an accessToken
- **plan_bus_route**: Calculate routes between points using the EMT network


## Installation & Usage

To install and use the **EMT Madrid (Open Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emt-madrid-open-data](https://vinkius.com/mcp/emt-madrid-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
