# Mato Grosso do Sul Open Data MCP Server

Access public datasets from the state of Mato Grosso do Sul (Brazil) — list packages, search datastores, and query public records via SQL.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mato-grosso-do-sul-open-data)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect to the **Mato Grosso do Sul (MS) Open Data Portal** to explore and analyze public information from the Brazilian state. This server allows AI agents to programmatically access datasets, organizations, and specific resource records.

### What you can do

- **Datasets & Packages** — List all available public data packages and retrieve detailed metadata using `list_packages` and `get_package`.
- **Resource Inspection** — Drill down into specific files or links within datasets to understand their structure with `get_resource`.
- **DataStore Search** — Filter and search through actual records in CSVs or spreadsheets directly using `datastore_search`.
- **SQL Queries** — Execute complex SQL statements on DataStore resources for advanced data analysis with `datastore_search_sql`.
- **Organizational Context** — List the government organizations and groups responsible for the data via `list_organizations` and `list_groups`.

### How it works

1. Subscribe to this server
2. Enter your Mato Grosso do Sul Data Portal API Key
3. Start querying public state data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — instantly retrieve and filter state records without manual downloads
- **Researchers** — automate the collection of public metadata and resource links
- **Developers** — integrate real-time public data into applications using SQL queries


## Available Tools
- **datastore_search_sql**: Execute a SQL query on DataStore resources
- **datastore_search**: Search data in a DataStore resource
- **get_package**: Get details of a specific dataset package
- **get_resource**: Get details of a specific resource
- **list_groups**: List all groups
- **list_organizations**: List all organizations
- **list_packages**: List all dataset packages


## Installation & Usage

To install and use the **Mato Grosso do Sul Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mato-grosso-do-sul-open-data](https://vinkius.com/mcp/mato-grosso-do-sul-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
