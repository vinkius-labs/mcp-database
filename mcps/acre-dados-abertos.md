# Acre Dados Abertos MCP Server

Access open data from the State of Acre, Brazil — explore datasets, organizations, and thematic groups directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/acre-dados-abertos)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect to the **Acre Dados Abertos** portal to query public information from the State of Acre. This server allows AI agents to browse, search, and analyze government datasets, organizational structures, and thematic groups.

### What you can do

- **Dataset Discovery** — List and search for specific packages (datasets) like municipal GDP, environmental data, or demographic statistics.
- **Metadata Inspection** — Fetch detailed metadata for packages and individual resources (files) to understand data provenance and formats.
- **Thematic Exploration** — Browse data organized by thematic groups (e.g., economy, health, education) or by the specific government organizations that publish them.
- **Deep Data Querying** — Search and filter records directly within tabular resources (Datastore) like CSV files without downloading the entire dataset.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Acre API Key if you have one for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and sample public datasets for research and reporting
- **Journalists** — verify government figures and find public records through natural language
- **Developers** — integrate real-time public data into applications using the Datastore search capabilities


## Available Tools
- **get_group**: Get details for a specific group
- **get_package**: Get detailed metadata for a specific dataset (package)
- **get_resource**: Get metadata for a specific resource
- **list_groups**: List all thematic groups
- **list_organizations**: List all organizations
- **list_packages**: List all dataset (package) names
- **search_datastore**: Search and filter records within a tabular resource (Datastore)
- **search_packages**: Search for datasets (packages)


## Installation & Usage

To install and use the **Acre Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acre-dados-abertos](https://vinkius.com/mcp/acre-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
