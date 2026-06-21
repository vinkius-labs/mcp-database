# SurrealDB MCP Server

Manage SurrealDB instances — execute SurrealQL, query tables, and manage records directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/surrealdb)

## Overview
**Category:** databases
**Tools Count:** 16

## Description
Connect your **SurrealDB** database to any AI agent and take full control of your data layer through natural conversation.

### What you can do

- **SurrealQL Execution** — Run raw SurrealQL statements using the `execute_sql` tool for complex queries and logic.
- **Record Management** — Create, update, and modify records in specific tables with tools like `create_record`, `update_record`, or `modify_record`.
- **Table Operations** — Quickly `select_all` or `delete_all` records from a target table to manage your data at scale.
- **Health Monitoring** — Check server status and health metrics using `get_status` and `get_health` to ensure uptime.
- **Data Portability** — Use `import_sql` and `export_data` to move information in and out of your instance seamlessly.

### How it works

1. Subscribe to this server
2. Enter your SurrealDB URL and credentials (NS, DB, and Auth)
3. Start managing your multi-model database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — test queries and inspect database state without switching windows.
- **Data Engineers** — perform quick data migrations or schema inspections via natural language.
- **Product Managers** — query business metrics directly from the database using SurrealQL.


## Available Tools
- **create_specific_record**: Create a specific record
- **delete_all**: Delete all records in a table
- **delete_record**: Delete a specific record
- **export_data**: Export data
- **get_health**: Check SurrealDB health
- **import_sql**: Import SurrealQL queries
- **modify_all**: Modify all records in a table (Merge)
- **modify_record**: Modify a specific record (Merge)
- **select_all**: Select all records in a table
- **select_record**: Select a specific record
- **create_record**: Create a record with a random ID
- **execute_sql**: Can pass variables via URL query parameters.

Execute SurrealQL statements
- **get_status**: Check SurrealDB web server status
- **update_all**: Update all records in a table
- **update_record**: Update a specific record
- **get_version**: Get SurrealDB version


## Installation & Usage

To install and use the **SurrealDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surrealdb](https://vinkius.com/mcp/surrealdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
