# Dades Obertes Catalunya MCP Server

Access Catalonia's Open Data portal — search catalogs and query datasets using SoQL to extract public information directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dades-obertes-catalunya)

## Overview
**Category:** data-analytics
**Tools Count:** 2

## Description
Unlock the power of **Dades Obertes Catalunya**, the official open data platform of the Government of Catalonia. This MCP server allows your AI agent to browse thousands of public datasets and perform complex queries through natural conversation.

### What you can do

- **Catalog Discovery** — Search for datasets by keywords, categories, or tags to find relevant public information using the `search_catalog` tool.
- **Advanced Querying** — Use SoQL (Socrata Query Language) via `query_dataset` to filter, select specific columns, and sort data from any dataset using its 4x4 identifier.
- **Data Analysis** — Group results and perform full-text searches across entire datasets to extract insights on health, transport, economy, and more.
- **Pagination & Limits** — Efficiently handle large datasets with built-in support for limits and offsets to browse records systematically.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Socrata App Token for higher rate limits
3. Start querying Catalan public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly pull public statistics into your workflow without manual CSV downloads
- **Researchers** — find and cross-reference government data on demographics, environment, or urban planning
- **Developers** — test data queries and explore API structures directly through natural language


## Available Tools
- **query_dataset**: g., abcd-1234). Supports SoQL parameters like $select, $where, $limit.

Query a specific dataset using SoQL parameters
- **search_catalog**: Returns dataset identifiers needed for the query_dataset tool.

Search the Dades Obertes Catalunya catalog for datasets


## Installation & Usage

To install and use the **Dades Obertes Catalunya** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dades-obertes-catalunya](https://vinkius.com/mcp/dades-obertes-catalunya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
