# IBAMA Dados Abertos MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ibama-dados-abertos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ibama-dados-abertos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ibama-dados-abertos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Brazilian environmental open data — query datasets, inspect resources, and analyze environmental metrics directly from IBAMA's official portal.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBAMA Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'licenciamento ambiental' and show the top 5 results."

**🤖 AI Agent:**
> I found several datasets. The top results include: 'Licenciamento Ambiental Federal', 'Empreendimentos Licenciados', and 'Processos de Licenciamento'. Which one would you like to explore?

---

**👤 You:**
> "List all thematic groups available in the IBAMA portal."

**🤖 AI Agent:**
> The available thematic groups are: 'Administrativo', 'Autorizações', 'Cadastro', 'Fiscalização', 'Flora', 'Fauna', and 'Qualidade Ambiental'.

---

**👤 You:**
> "Query the resource 'd34981d9-24c6-4d86-96c3-997d0e0d7f62' for records where the year is 2023."

**🤖 AI Agent:**
> I've queried the DataStore for that resource. I found 150 records for the year 2023. Here are the first few entries showing the location and type of environmental occurrence...


## Installation & Usage

To install and use the **IBAMA Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibama-dados-abertos](https://vinkius.com/mcp/ibama-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
