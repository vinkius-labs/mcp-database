# MyScale (SQL Vector Database API) MCP Server

Manage MyScale vector databases via SQL — execute queries, perform vector searches, and manage indices directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/myscale-sql-vector-database-api)

## Overview
**Category:** databases
**Tools Count:** 6

## Description
Connect your **MyScale** cluster to any AI agent to manage high-performance vector data using familiar SQL syntax. MyScale combines the power of ClickHouse with advanced vector search capabilities.

### What you can do

- **SQL Execution** — Run arbitrary SQL queries including SELECT, INSERT, and ALTER directly on your cluster via `execute_sql_query`.
- **Vector Search** — Perform similarity searches using the `vector_search` tool which automatically handles distance functions and SQL construction.
- **Index Management** — Create and monitor specialized vector indices (MSTG, ScaNN, HNSW) using `create_vector_index` and `check_index_status`.
- **Schema Control** — Quickly set up new environments with `create_vector_table`, defining dimensions and constraints through natural language.
- **Connectivity Checks** — Instantly verify your database status and credentials with `ping_cluster`.

### How it works

1. Subscribe to this server
2. Enter your MyScale Cluster URL, Username, and Password
3. Start managing your vector data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Engineers** — test vector search parameters and inspect data distributions without leaving the chat
- **Data Scientists** — manage RAG (Retrieval-Augmented Generation) backends and monitor index health in real-time
- **Backend Developers** — perform database maintenance and schema updates using natural language commands


## Available Tools
- **check_index_status**: vector_indices table to monitor the build status of vector indices (Built, InProgress, Error).

Check the status of vector indices
- **create_vector_index**: ADD VECTOR INDEX statement.

Create a vector index on a table
- **create_vector_table**: Create a new table with a vector column
- **execute_sql_query**: For SELECT queries, FORMAT JSON is automatically appended.

Execute an arbitrary SQL query on MyScale
- **ping_cluster**: Check MyScale cluster connectivity
- **vector_search**: Automatically constructs the SQL query.

Perform a vector similarity search


## Installation & Usage

To install and use the **MyScale (SQL Vector Database API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/myscale-sql-vector-database-api](https://vinkius.com/mcp/myscale-sql-vector-database-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
