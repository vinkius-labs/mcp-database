# RisingWave (Streaming Database) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/risingwave-streaming-database)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/risingwave-streaming-database-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/risingwave-streaming-database-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage your RisingWave streaming database — execute SQL, ingest events, and monitor tables, materialized views, sources, and sinks directly from any AI agent.

## Description
Connect your **RisingWave** streaming database to any AI agent and take full control of your real-time data processing workflows through natural conversation.

### What you can do

- **SQL Execution** — Run DDL and DML statements like CREATE, SELECT, and INSERT directly via the HTTP API
- **Event Ingestion** — Stream JSON data into your tables instantly using the dedicated Events API
- **Catalog Discovery** — List all tables, materialized views, external sources, and sinks to understand your data topology
- **Real-time Monitoring** — Inspect the state of your streaming pipelines and materialized views without leaving your workspace

### How it works

1. Subscribe to this server
2. Enter your RisingWave URL
3. Start managing your streaming database from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — quickly verify streaming logic and inspect materialized views during development
- **Backend Developers** — ingest test events and query tables directly from the code editor
- **Analytics Teams** — explore available data sources and sinks to build real-time dashboards


## Available Tools
- **execute_sql**: Execute a SQL statement on RisingWave
- **ingest_events**: Body can be a single JSON object or an array of objects.

Ingest events into a RisingWave table
- **list_materialized_views**: rw_materialized_views to list all materialized views.

List materialized views in RisingWave
- **list_sinks**: rw_sinks to list all data sinks.

List sinks in RisingWave
- **list_sources**: rw_sources to list all external data sources.

List sources in RisingWave
- **list_tables**: tables to list user tables.

List tables in RisingWave


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RisingWave (Streaming Database)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the materialized views currently active in RisingWave."

**🤖 AI Agent:**
> I've retrieved the catalog. You have 3 active materialized views: 'daily_sales_summary', 'user_login_stats', and 'realtime_inventory_levels'. Which one would you like to inspect?

---

**👤 You:**
> "Ingest this JSON event into the 'user_activity' table: {"user_id": 123, "action": "login"}."

**🤖 AI Agent:**
> I've successfully sent the event to the 'user_activity' table via the RisingWave Events API. The data is now available for streaming processing.

---

**👤 You:**
> "Show me all external data sinks configured in the system."

**🤖 AI Agent:**
> Querying the catalog... I found 2 configured sinks: 's3_archived_logs' (S3) and 'postgres_reporting_db' (JDBC).


## Installation & Usage

To install and use the **RisingWave (Streaming Database)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/risingwave-streaming-database](https://vinkius.com/mcp/risingwave-streaming-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
