# SurrealDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/surrealdb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/surrealdb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/surrealdb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage SurrealDB instances — execute SurrealQL, query tables, and manage records directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SurrealDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the health and version of my SurrealDB server."

**🤖 AI Agent:**
> I've checked your instance. The server is healthy (200 OK) and currently running SurrealDB version 2.1.0.

---

**👤 You:**
> "Select all records from the 'users' table."

**🤖 AI Agent:**
> I've retrieved all records from the 'users' table. There are 3 records: 'user:admin', 'user:john_doe', and 'user:jane_smith'. Would you like to see the details of a specific one?

---

**👤 You:**
> "Execute a SurrealQL query to find all posts where status is 'published'."

**🤖 AI Agent:**
> Running the SurrealQL query... I found 12 posts with the 'published' status. The most recent one is 'post:mcp-guide' created on 2023-10-27.


## Installation & Usage

To install and use the **SurrealDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surrealdb](https://vinkius.com/mcp/surrealdb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
