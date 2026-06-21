# EPA Envirofacts (Environmental Data) MCP Server

Access US environmental data including UV forecasts, facility information, and toxic release inventories directly from the EPA.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-envirofacts-environmental-data)

## Overview
**Category:** government-public-data
**Tools Count:** 6

## Description
Connect to the **EPA Envirofacts** database to query a wealth of environmental information directly from the United States Environmental Protection Agency.

### What you can do

- **UV Index Forecasts** — Retrieve hourly and daily UV Index forecasts by ZIP code or City/State to monitor solar radiation levels.
- **Facility Research** — Query the Toxic Release Inventory (TRI) and Superfund (SEMS) databases to find environmental records for specific sites.
- **Advanced Data Exploration** — Use GraphQL to perform complex queries, aggregations, and cross-table analysis across the EPA's DMAP API.
- **Flexible REST Queries** — Search any table in the Envirofacts database with custom filters, operators, and pagination.
- **Public Data Access** — Access official government records on air, water, and waste without complex registration.

### How it works

1. Subscribe to this server
2. No private API key is required for public EPA data access
3. Start querying environmental metrics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Researchers** — quickly pull data from TRI or SEMS for impact analysis and reporting
- **Health & Safety Professionals** — monitor UV radiation levels to provide accurate safety guidance
- **Developers & Data Scientists** — integrate official government environmental data into applications via GraphQL or REST


## Available Tools
- **graphql_query**: Query EPA Envirofacts using GraphQL
- **rest_query**: Use program.table format (e.g., tri.tri_facility).

Query EPA Envirofacts REST API
- **uv_daily_city_state**: Get daily UV Index forecast by City and State
- **uv_daily_zip**: Get daily UV Index forecast by ZIP code
- **uv_hourly_city_state**: Get hourly UV Index forecast by City and State
- **uv_hourly_zip**: Get hourly UV Index forecast by ZIP code


## Installation & Usage

To install and use the **EPA Envirofacts (Environmental Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-envirofacts-environmental-data](https://vinkius.com/mcp/epa-envirofacts-environmental-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
