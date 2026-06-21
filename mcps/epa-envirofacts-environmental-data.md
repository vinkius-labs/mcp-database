# EPA Envirofacts (Environmental Data) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-envirofacts-environmental-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/epa-envirofacts-environmental-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/epa-envirofacts-environmental-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access US environmental data including UV forecasts, facility information, and toxic release inventories directly from the EPA.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EPA Envirofacts (Environmental Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the hourly UV forecast for ZIP code 90210?"

**🤖 AI Agent:**
> I've retrieved the hourly UV forecast for Beverly Hills (90210). The index starts at 1 in the morning, peaks at 7 (High) around 1:00 PM, and decreases toward the evening. Would you like the daily summary as well?

---

**👤 You:**
> "Search the 'sems.envirofacts_site' table for facilities in the city of 'Miami'."

**🤖 AI Agent:**
> Querying the SEMS database... I found several environmental sites in Miami. Notable entries include the 'Miami Drum Services' and 'Munisport Landfill'. Would you like the full details for any of these site IDs?

---

**👤 You:**
> "Run a GraphQL query to count TRI facilities by state."

**🤖 AI Agent:**
> Executing the GraphQL aggregation... The query returned the facility counts. For example, Texas has 1,542 facilities and California has 1,210. Would you like me to list the counts for all states?


## Installation & Usage

To install and use the **EPA Envirofacts (Environmental Data)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-envirofacts-environmental-data](https://vinkius.com/mcp/epa-envirofacts-environmental-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
