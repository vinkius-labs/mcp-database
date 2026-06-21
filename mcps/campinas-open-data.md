# Campinas Open Data MCP Server

Access public data from Campinas, Brazil — search datasets, resources, and city organizations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/campinas-open-data)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect to the **Campinas Open Data Portal** (CKAN) and explore a wealth of public information from one of Brazil's major cities through natural conversation.

### What you can do

- **Dataset Discovery** — Search for specific packages related to health, education, finance, or transport using keywords.
- **Metadata Inspection** — Retrieve full metadata for datasets and individual resources (files) to understand data structures.
- **Organizational Mapping** — List all city departments and organizations that provide public data.
- **Thematic Exploration** — Browse data by groups (e.g., 'Saúde', 'Educação') or tags to find relevant information quickly.
- **Resource Access** — Get direct links and metadata for CSVs, PDFs, and APIs hosted on the portal.

### How it works

1. Subscribe to this server
2. Enter your Campinas Portal API Key (optional for public data, required for restricted access)
3. Start querying city data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find datasets for urban studies or public policy analysis.
- **Developers** — inspect API resources and data schemas without leaving the code editor.
- **Journalists & Citizens** — explore public spending and city metrics through simple questions.


## Available Tools
- **list_groups**: g., Education, Health).

List thematic groups
- **list_organizations**: List organizations providing data
- **list_packages**: List all dataset names
- **search_packages**: Search for datasets matching specific criteria
- **get_package**: Get full metadata for a specific dataset
- **search_resources**: g., name:financeiro).

Search for resources based on fields
- **get_resource**: Get metadata for a specific resource
- **list_tags**: List all tags used across the portal


## Installation & Usage

To install and use the **Campinas Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/campinas-open-data](https://vinkius.com/mcp/campinas-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
