# EPA Envirofacts (Environmental Data) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/epa-envirofacts-environmental-data)
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


## Available Tools (6)
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


## ❓ FAQ

**Q: How can I check the UV Index for a specific location?**
Use the `uv_hourly_zip` or `uv_hourly_city_state` tools. Simply provide a 5-digit US ZIP code or the city name and 2-letter state abbreviation to receive the latest hourly forecast data.

**Q: Can I search for specific facilities in the EPA database?**
Yes! Use the `rest_query` tool. You can specify tables like 'tri.tri_facility' or 'sems.envirofacts_site' and apply filters using operators like 'equals' or 'contains' to find specific sites and their environmental records.

**Q: Does this server support complex data aggregations?**
Absolutely. The `graphql_query` tool allows you to execute custom GraphQL strings to perform advanced data fetching, aggregations, and subqueries across the EPA's DMAP API infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/epa-envirofacts-environmental-data](https://vinkius.com/mcp/epa-envirofacts-environmental-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EPA Envirofacts (Environmental Data)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `epa-envirofacts-environmental-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EPA Envirofacts (Environmental Data)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "epa-envirofacts-environmental-data": {
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
