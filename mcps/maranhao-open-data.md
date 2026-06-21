# Maranhão Open Data MCP Server

Access public datasets from Maranhão, Brazil — search packages, inspect resources, and query the datastore via SQL.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/maranhao-open-data)

## Overview
**Category:** knowledge-management
**Tools Count:** 6

## Description
Connect to the **Maranhão Open Data Portal** to explore government transparency data directly through your AI agent. This server interfaces with the state's CKAN-based infrastructure to provide real-time access to public information.

### What you can do

- **Dataset Discovery** — List all available packages or search for specific topics like education, health, or finance using `list_packages` and `search_packages`.
- **Metadata Inspection** — Retrieve detailed metadata for datasets and specific resources (CSV, PDF, API endpoints) with `get_package` and `get_resource`.
- **Data Exploration** — Search within specific resource rows using `search_datastore` or execute complex SQL queries against the DataStore for deep analysis with `search_datastore_sql`.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Maranhão API Key for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Journalists** — quickly find and analyze government spending, social indicators, and public contracts.
- **Developers** — integrate public data into applications without manually browsing the portal.
- **Data Analysts** — run SQL queries directly on government datasets to generate insights and reports.


## Available Tools
- **get_package**: Retrieve dataset metadata
- **get_resource**: g., a CSV file or API endpoint within a dataset).

Retrieve resource metadata
- **list_packages**: List all datasets (packages) on the portal
- **search_datastore_sql**: Execute SQL query against the DataStore
- **search_datastore**: Search within a resource in the DataStore
- **search_packages**: Search for datasets


## Installation & Usage

To install and use the **Maranhão Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maranhao-open-data](https://vinkius.com/mcp/maranhao-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
