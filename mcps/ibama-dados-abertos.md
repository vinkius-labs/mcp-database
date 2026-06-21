# IBAMA Dados Abertos MCP Server

Access Brazilian environmental open data — query datasets, inspect resources, and analyze environmental metrics directly from IBAMA's official portal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ibama-dados-abertos)

## Overview
**Category:** data-analytics
**Tools Count:** 9

## Description
Connect to the **IBAMA Open Data Portal** (CKAN) to explore and analyze critical environmental information from Brazil. This server allows any AI agent to navigate through thousands of public records regarding environmental licensing, federal technical registries, and inspection activities.

### What you can do

- **Dataset Discovery** — Search and list datasets related to deforestation, wildlife, flora, and environmental fines using keywords or thematic groups.
- **Metadata Inspection** — Fetch detailed metadata for specific datasets and resources to understand data provenance and update frequency.
- **Direct Data Querying** — Use the DataStore integration to query CSV and tabular data directly using filters and SQL-like parameters without downloading large files.
- **Organizational Mapping** — Explore the structure of IBAMA departments and the specific data they publish.

### How it works

1. Subscribe to this server
2. (Optional) Provide your IBAMA/CKAN API Key for higher rate limits
3. Start querying environmental data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Environmental Researchers** — quickly find and filter datasets for academic or scientific studies.
- **Data Journalists** — extract specific records about environmental infractions or licensing status for reporting.
- **Policy Analysts** — monitor public data updates to track environmental enforcement trends in Brazil.


## Available Tools
- **datastore_search**: Query CSV/Tabular data directly
- **list_datasets**: List all dataset names
- **list_groups**: List all thematic groups
- **list_organizations**: g., IBAMA departments).

List all organizations
- **search_datasets**: Supports sorting and pagination.

Search for datasets matching a query string
- **search_resources**: Search for resources based on specific fields
- **show_dataset**: Show full metadata for a specific dataset
- **show_organization**: Show details and datasets of an organization
- **show_resource**: Show metadata for a specific resource


## Installation & Usage

To install and use the **IBAMA Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibama-dados-abertos](https://vinkius.com/mcp/ibama-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
