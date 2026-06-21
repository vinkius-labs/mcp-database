# Oracle Vector DB MCP Server

Run vector similarity searches on Oracle 23ai — execute VECTOR_DISTANCE queries, inspect schemas, list vector indexes, and query tables from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/oracle-vector-db)

## Overview
**Category:** industry-titans
**Tools Count:** 7

## Description
Bring your **Oracle Database 23ai** vector capabilities directly into your AI agent workflow. Run VECTOR_DISTANCE similarity searches, inspect table schemas, execute SQL queries, and manage vector indexes — all through natural conversation.

### What you can do

- **Vector Similarity Search** — Execute native Oracle 23ai VECTOR_DISTANCE queries with cosine or Euclidean metrics against any table with VECTOR columns
- **Schema Inspection** — List all tables in your schema and describe column types, spotting VECTOR-enabled columns for embedding storage
- **SQL Execution** — Run arbitrary SQL queries against Oracle via ORDS for ad-hoc analysis and data retrieval
- **Vector Index Management** — List all HNSW and IVF vector indexes instantiated across your tables
- **Table Statistics** — Get row counts and optimizer stats for capacity planning and query performance tuning
- **Version Check** — Verify your Oracle runtime version to confirm 23ai vector feature compatibility

### How it works

1. Subscribe to this server
2. Enter your Oracle ORDS URL, Schema, Username, and Password
3. Start querying your vector store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Enterprise data teams** — run vector searches against production Oracle databases without context-switching to SQL Developer
- **ML engineers** — test embedding queries on Oracle 23ai's native vector engine during RAG pipeline development
- **DBAs** — inspect vector indexes, table stats, and schema configurations through conversation


## Available Tools
- **list_tables**: List accessible tables in the current Oracle schema
- **describe_table**: Describe table columns and explicit data types including VECTORs
- **execute_sql_query**: WARNING: Output payload size is inherently limited, restrict rows fetched (FETCH FIRST 100 ROWS ONLY) to ensure stability.

Execute arbitrary SQL query against the Oracle runtime via ORDS
- **vector_search**: 1, -0.4, 0.5]` against a strict `VECTOR` column natively inside Oracle DB, sorting and fetching the nearest neighbors.

Execute Vector similarity search via Oracle 23ai native VECTOR_DISTANCE
- **list_vector_indexes**: List specialized AI Vector search indexes (HNSW, IVF) instantiated
- **table_stats**: Get table cardinality and optimizer statistics
- **get_database_version**: Get exact Oracle DB Runtime version banner


## Installation & Usage

To install and use the **Oracle Vector DB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oracle-vector-db](https://vinkius.com/mcp/oracle-vector-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
