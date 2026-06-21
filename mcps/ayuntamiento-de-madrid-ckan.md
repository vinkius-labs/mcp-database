# Ayuntamiento de Madrid (CKAN) MCP Server

Access Madrid's open data portal — list datasets, search for municipal information, and inspect resources from the city's CKAN repository.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ayuntamiento-de-madrid-ckan)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect to the official **Open Data portal of the Madrid City Council** and explore thousands of public datasets through natural conversation. This server interfaces with the city's CKAN repository to provide real-time access to municipal information.

### What you can do

- **Dataset Discovery** — List all available packages or search for specific topics like transport, environment, or budget using `list_packages` and `search_packages`.
- **Metadata Inspection** — Retrieve deep metadata for any dataset, including its maintainer, update frequency, and license using `get_package`.
- **Resource Access** — Identify specific files (CSV, JSON, XLS) within a dataset and fetch their individual metadata using `get_resource` or `search_resources`.
- **Organizational Mapping** — List all municipal departments and organizations that publish data to understand the source of the information using `list_organizations`.
- **Categorization** — Browse data by groups or tags to find related information across different city sectors using `list_groups` and `list_tags`.

### How it works

1. Subscribe to this server
2. Enter your API Key from the Madrid Data portal (if required for specific endpoints)
3. Start querying city data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect municipal datasets for urban research or trend analysis.
- **Developers** — retrieve resource IDs and metadata to integrate city data into applications without leaving the IDE.
- **Citizens & Researchers** — explore public information about Madrid's services, environment, and economy through simple questions.


## Available Tools
- **madrid_get_package**: Get full metadata for a specific dataset
- **madrid_get_resource**: Get metadata for a specific file/resource
- **madrid_list_groups**: List all categories/groups
- **madrid_list_organizations**: List municipal departments/organizations
- **madrid_list_packages**: List all dataset names in the portal
- **madrid_search_packages**: Supports filtering by tags, groups, etc.

Search for datasets matching a query
- **madrid_search_resources**: Search for resources matching specific criteria
- **madrid_list_tags**: List all tags used in the catalog


## Installation & Usage

To install and use the **Ayuntamiento de Madrid (CKAN)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ayuntamiento-de-madrid-ckan](https://vinkius.com/mcp/ayuntamiento-de-madrid-ckan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
