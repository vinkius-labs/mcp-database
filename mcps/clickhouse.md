# ClickHouse MCP Server

Query and manage ClickHouse databases — execute analytical SQL, monitor replication status, and manage schemas directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clickhouse)

## Overview
**Category:** brain-trust
**Tools Count:** 4

## Description
Connect your **ClickHouse** instance to any AI agent to perform lightning-fast OLAP queries and manage your data infrastructure through natural language.

### What you can do

- **Analytical Queries** — Execute read-only SELECT queries with automatic safety limits using the `select_query` tool.
- **Schema Management** — Create, alter, or drop tables and databases using the `execute_query` action for mutating operations.
- **Health Monitoring** — Instantly verify server availability with `ping` and check replication lag across clusters with `replicas_status`.
- **Performance Tuning** — Pass specific settings like `max_rows_to_read` or `max_execution_time` to optimize resource usage.

### How it works

1. Subscribe to this server
2. Enter your ClickHouse URL, Username, and Password
3. Start querying your big data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — quickly inspect table schemas and row counts without switching to a SQL IDE.
- **Analysts** — run complex aggregations and get instant summaries of large datasets.
- **DevOps** — monitor cluster health and replication status during maintenance or incidents.


## Available Tools
- **execute_query**: Execute a mutating query on ClickHouse
- **ping**: Check ClickHouse server health
- **replicas_status**: Check ClickHouse replica delay
- **select_query**: Automatically enforces readonly=1.

Execute a read-only SELECT query on ClickHouse


## Installation & Usage

To install and use the **ClickHouse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickhouse](https://vinkius.com/mcp/clickhouse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
