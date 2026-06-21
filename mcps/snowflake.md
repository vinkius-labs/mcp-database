# Snowflake MCP Server

Bring your absolute data cloud into your AI editor. Execute queries, list warehouses, and map complex schemas natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/snowflake)

## Overview
**Category:** industry-titans
**Tools Count:** 7

## Description
Connect your **Snowflake** AI Data Cloud with your AI agent to radically accelerate the way you query large datasets and audit cloud data warehouses. Navigate through deep hierarchical trees of databases, tables, and internal stages natively by chatting with your IDE. Keep your SQL robust by validating commands directly against the live engine.

### What you can do

- **Execute Queries in Chat** — Tell your bot to `execute_sql` based on human prompts or test new complex table joins safely right inside Cursor or Claude
- **Map Infrastructures** — Quickly retrieve spatial contexts by pulling `list_databases`, traversing downwards through `list_schemas` to target specific columns
- **Audit Compute Cost** — Keep a firm grip on active clusters running by auditing running instances using `list_warehouses`
- **Diagnose Operations** — Monitor long-tail data workloads or data engineering pipelines using the `get_query_status` method asynchronously

### How it works

1. Subscribe to this AI integration server
2. Introduce your explicit Snowflake Account identifier (e.g. `abc123.us-east-1`)
3. Inject your Snowflake OAuth token or JWT Token (key pair) authentication string
4. Ask Claude or Cursor to look into the Sales Database schema

Stop juggling browser instances to paste a quick query in Snowflake Snowsight. Stay strictly inside your local codebase while examining the exact table data types.

### Who is this for?

- **Data Engineers** — validate that raw datasets correctly land in internal environments (`list_stages`) straight from your IDE window
- **Analytics Engineers / dbt** — generate highly accurate SQL modeling by letting your agent examine the `list_tables` definitions live
- **Software Architects** — write an agentic script pulling raw diagnostic query metrics without downloading hefty SDK kits locally


## Available Tools
- **list_databases**: Lists all databases in the Snowflake account
- **list_schemas**: Lists all schemas within a specific database
- **list_tables**: Lists all tables within a specific schema
- **execute_sql**: Prefers read-only statements whenever possible.

Executes a SQL query on Snowflake
- **list_warehouses**: Lists all virtual warehouses
- **list_stages**: Lists all internal and external stages
- **get_query_status**: Retrieves the status of an asynchronous query


## Installation & Usage

To install and use the **Snowflake** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snowflake](https://vinkius.com/mcp/snowflake)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
