# ElectricSQL (Sync Engine) MCP Server

Sync Postgres data to your AI agent in real-time using ElectricSQL's HTTP Sync API — fetch shapes, stream updates, and query subsets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/electricsql-sync-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 2

## Description
Connect your **ElectricSQL** sync engine to any AI agent to stream data directly from Postgres into your conversation context. This server leverages the Electric HTTP Sync API to fetch 'shapes' of data efficiently.

### What you can do

- **Real-time Sync** — Fetch data from Postgres tables with support for initial snapshots and incremental updates using log offsets.
- **Shape Management** — Define specific subsets of data (shapes) using SQL-like WHERE clauses and precise column selection.
- **Live Streaming** — Enable long-polling or Server-Sent Events (SSE) to keep your agent updated as data changes in the database.
- **Complex Filtering** — Use POST-based subset snapshots to handle complex WHERE clauses without hitting URL length limits.
- **Pagination & Limits** — Efficiently browse large datasets with built-in limit, offset_rows, and order_by support.

### How it works

1. Subscribe to this server
2. Provide your Electric Service URL (e.g., your local or cloud Electric endpoint)
3. Start querying your Postgres data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — build AI-powered tools that need live access to application data without complex backend plumbing.
- **Data Engineers** — inspect and sync specific database 'shapes' for analysis or debugging via natural language.
- **Product Teams** — monitor real-time system state or user activity directly within the AI chat interface.


## Available Tools
- **get_shape**: Use offset=-1 for initial sync.

Sync a shape of data out of Postgres via GET
- **post_shape**: Sync a shape of data out of Postgres via POST (Subset Snapshots)


## Installation & Usage

To install and use the **ElectricSQL (Sync Engine)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/electricsql-sync-engine](https://vinkius.com/mcp/electricsql-sync-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
