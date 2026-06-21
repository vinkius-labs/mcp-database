# Aragón Open Data MCP Server

Access public data from the Government of Aragón — query datasets, preview views, and explore the CKAN catalog directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aragon-open-data)

## Overview
**Category:** knowledge-management
**Tools Count:** 15

## Description
Connect to the **Aragón Open Data** portal and unlock a wealth of public information from the Government of Aragón. This MCP server allows your AI agent to browse, search, and analyze regional datasets, statistical views, and organizational metadata through natural language.

### What you can do

- **Data Exploration** — List all available views and datasets from the GA_OD_Core and CKAN catalogs.
- **Deep Data Preview** — Fetch and preview actual records from specific views or resources with support for filtering and pagination.
- **Schema Inspection** — Understand the structure of data by retrieving column names and data types for any specific view.
- **Advanced Search** — Use Solr-powered queries to find specific datasets, tags, or organizations within the public catalog.
- **Publisher Insights** — Retrieve detailed information about the organizations and themes (groups) that publish data in the region.

### How it works

1. Subscribe to this server
2. Enter your Aragón Open Data API Key (optional for public endpoints)
3. Start querying public records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and preview regional statistics without manual CSV downloads
- **Developers** — inspect API schemas and data structures directly from the code editor
- **Researchers & Journalists** — search for public records and government transparency data through conversation


## Available Tools
- **count_datasets**: Get total dataset count
- **get_organization**: Get publisher/organization details
- **get_dataset**: Get dataset details
- **get_tag**: Get tag details
- **list_groups**: List all themes/groups
- **list_organizations**: List all publishers/organizations
- **list_datasets**: List all datasets (packages)
- **list_tags**: List all tags
- **list_views**: List all available views in Aragón Open Data
- **most_downloaded_datasets**: Get most downloaded datasets
- **newest_datasets**: Get newest datasets
- **preview_data**: By default, it returns the first 1000 records.

Preview data from a view or resource
- **query_sparql**: Supports ontologies like EI2A, Aragopedia, ELI, and DataCube.

Execute a SPARQL query
- **search_datasets**: Search for datasets
- **show_columns**: Get information about columns for a specific view


## Installation & Usage

To install and use the **Aragón Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aragon-open-data](https://vinkius.com/mcp/aragon-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
