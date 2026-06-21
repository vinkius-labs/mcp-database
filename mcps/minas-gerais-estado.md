# Minas Gerais (Estado) MCP Server

Access the official Open Data Portal of the State of Minas Gerais, Brazil. Query datasets, organizations, and public resources directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/minas-gerais-estado)

## Overview
**Category:** data-management
**Tools Count:** 10

## Description
Connect to the **Minas Gerais State Open Data Portal** to explore a vast repository of public information. This server allows AI agents to programmatically browse, search, and retrieve metadata from one of Brazil's most comprehensive transparency portals.

### What you can do

- **Dataset Discovery** — List all available packages or search for specific datasets related to health, education, or finance using `list_packages` and `search_packages`.
- **Organizational Insights** — Explore the structure of the state government by listing departments and viewing their specific datasets via `list_organizations` and `get_organization`.
- **Resource Access** — Identify specific files (CSV, PDF, XLS) within datasets and retrieve their metadata using `get_resource` and `search_resources`.
- **Categorized Browsing** — Navigate data through thematic groups (categories) or tags to find exactly what you need with `list_groups` and `list_tags`.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Minas Gerais Portal API Key for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets for research and reporting
- **Journalists** — automate the discovery of government transparency data and organizational structures
- **Developers** — integrate official state data into applications without manual portal navigation


## Available Tools
- **list_groups**: List all groups (categories)
- **get_group**: Get details and datasets of a group
- **list_organizations**: List all organizations
- **get_organization**: Get details and datasets of an organization
- **list_packages**: List all dataset names in the portal
- **search_packages**: Search for datasets matching specific criteria
- **get_package**: Get full metadata of a specific dataset
- **search_resources**: Search for resources matching a query
- **get_resource**: Get metadata of a specific resource (file)
- **list_tags**: List all tags used in the portal


## Installation & Usage

To install and use the **Minas Gerais (Estado)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/minas-gerais-estado](https://vinkius.com/mcp/minas-gerais-estado)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
