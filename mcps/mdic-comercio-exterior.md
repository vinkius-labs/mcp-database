# MDIC (Comércio Exterior) MCP Server

Access Brazilian foreign trade data from MDIC — list datasets, search for trade packages, and query the datastore for export/import statistics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mdic-comercio-exterior)

## Overview
**Category:** data-analytics
**Tools Count:** 5

## Description
Connect to the **MDIC (Ministry of Development, Industry, Trade and Services)** open data portal to analyze Brazilian foreign trade metrics directly through your AI agent.

### What you can do

- **Dataset Discovery** — List and search through all available trade packages (datasets) like 'comex-stat' or 'exportacao-municipios'
- **Metadata Inspection** — Get detailed descriptions, tags, and resource lists for specific trade datasets
- **Direct Data Querying** — Use the Datastore search to filter and retrieve specific rows from CSV resources using SQL-like parameters
- **Resource Management** — Access individual file metadata and download links for trade statistics

### How it works

1. Subscribe to this server
2. (Optional) Provide an API key if required by your specific endpoint for higher rate limits
3. Start querying Brazilian trade data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly fetch trade volumes and export trends without manual downloads
- **Economists** — analyze official government trade data using natural language queries
- **Business Intelligence Leads** — integrate official Brazilian trade statistics into automated reports and dashboards


## Available Tools
- **get_package**: Get detailed metadata for a specific dataset (package)
- **get_resource**: Get metadata for a specific resource (data file)
- **list_packages**: List all datasets (packages) available in the MDIC portal
- **search_datastore**: Query data directly from a resource stored in the Datastore
- **search_packages**: g., "comex", "exportação").

Search for datasets matching a specific query string


## Installation & Usage

To install and use the **MDIC (Comércio Exterior)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mdic-comercio-exterior](https://vinkius.com/mcp/mdic-comercio-exterior)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
