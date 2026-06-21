# EMT Madrid (Open Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emt-madrid-open-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/emt-madrid-open-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/emt-madrid-open-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access real-time Madrid public transport data: bus arrivals, BiciMAD bike status, and route planning via EMT Open Data.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EMT Madrid (Open Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the bus arrival times for stop ID 72?"

**🤖 AI Agent:**
> I've checked stop 72. Line 19 is arriving in 3 minutes, and Line 51 is estimated in 8 minutes. Would you like to check another stop?

---

**👤 You:**
> "List all BiciMAD stations and their current bike availability."

**🤖 AI Agent:**
> Fetching BiciMAD status... I found 600+ stations. For example, Station 'Puerta del Sol' has 12 bikes available and 15 free docks. Do you have a specific area in mind?

---

**👤 You:**
> "Plan a bus route starting from stop 1022."

**🤖 AI Agent:**
> Calculating routes from stop 1022... You can take Line 27 towards Plaza de Castilla. The next departure is in 5 minutes. Where is your final destination?


## Installation & Usage

To install and use the **EMT Madrid (Open Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emt-madrid-open-data](https://vinkius.com/mcp/emt-madrid-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
