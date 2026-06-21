# ClickHouse (Vector Search) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickhouse-vector-search)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clickhouse-vector-search-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clickhouse-vector-search-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage vector embeddings and SQL via ClickHouse — list databases, execute SQL, and perform high-speed vector searches directly from any AI agent.

## Description
Connect your **ClickHouse** cluster to any AI agent and take full control of your analytical and vector data through natural conversation.

### What you can do

- **Schema Management** — List databases and tables, and inspect deep column schemas including specialized Array(Float32) vector types
- **SQL Execution** — Push arbitrary DML, DDL, or SELECT queries to your cluster to manage data and generate real-time reports
- **Vector Search** — Identify mathematical distance traces using cosineDistance or L2Distance metrics for high-dimensional semantic search
- **Cluster Monitoring** — Extract internal structural states, row counts, and compression ratios to audit cluster health
- **Capability Auditing** — Check instance versions and binary limits to identify exact capability branches like HNSW support

### How it works

1. Subscribe to this server
2. Enter your ClickHouse URL (Cloud or self-hosted), Username, and Password
3. Start querying your analytical data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — generate complex analytical reports and execute SQL queries using natural language
- **AI Developers** — test and debug vector similarity searches and semantic matching without writing boilerplate code
- **Database Administrators** — monitor table statistics, compression ratios, and cluster versions across environments
- **Product Teams** — quickly verify analytical data and vector distributions during the prototyping phase


## Available Tools
- **list_databases**: Identify bounded logical arrays managing top-level ClickHouse schemas
- **list_tables**: Retrieve the exact structural matching verifying table limits inside a database
- **describe_table**: Perform structural extraction of properties driving active column schemas
- **execute_sql**: Provision a highly-available SQL execution pushing arbitrary arbitrary DML/DDL or SELECTs
- **vector_search**: Identify explicit mathematical distance traces routing Vector Embeddings
- **get_table_stats**: Extracts explicitly attached internal structural states pulling cluster health
- **get_version**: g. HNSW support).

Identify precise active cluster limits spanning the execution runtime


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickHouse (Vector Search)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all databases in my ClickHouse cluster"

**🤖 AI Agent:**
> I found 4 databases: 'default', 'analytics_prod', 'vector_store', and 'system'. Which one would you like to explore?

---

**👤 You:**
> "Find the top 5 most similar records in table 'embeddings' using this vector: [0.1, 0.5, -0.2]"

**🤖 AI Agent:**
> Vector search complete! I found 5 matches in 'analytics_prod.embeddings'. The top match has a cosineDistance of 0.045. Would you like to see the associated metadata for these records?

---

**👤 You:**
> "Get table stats for 'analytics_prod.sales_data'"

**🤖 AI Agent:**
> Stats for 'sales_data': 1.2M rows, 450MB total size, 4.2x compression ratio. The table is currently healthy and responsive.


## Installation & Usage

To install and use the **ClickHouse (Vector Search)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickhouse-vector-search](https://vinkius.com/mcp/clickhouse-vector-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
