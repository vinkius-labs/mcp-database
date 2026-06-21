# Región de Murcia Datos Abiertos MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/region-de-murcia-datos-abiertos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/region-de-murcia-datos-abiertos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/region-de-murcia-datos-abiertos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the official open data portal of the Region of Murcia (Spain) to query datasets, organizations, and public statistics.

## Description
Connect your AI agent to the **Región de Murcia Datos Abiertos** portal. This MCP server provides direct access to the CKAN-based catalog of the regional government of Murcia, Spain, allowing you to explore a wealth of public information.

### What you can do

- **Dataset Discovery** — Search through thousands of public datasets using keywords or list all available identifiers in the catalog.
- **Detailed Metadata** — Retrieve complete metadata for specific datasets, including descriptions, formats, and resource links.
- **Organizational Insights** — List and explore the various government organizations and groups that publish data on the portal.
- **Trend Tracking** — Instantly fetch the most recently updated or the most viewed datasets to stay informed on regional trends.
- **Public Transparency** — Access data regarding economy, environment, demographics, and infrastructure directly through natural language.

### How it works

1. Subscribe to this server
2. Enter your Murcia API Key (optional for public data, but recommended for higher rate limits)
3. Start querying Spanish regional data from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly find and inspect regional statistics without manual portal navigation
- **Researchers & Students** — gather public data for academic or social studies via simple conversation
- **Developers** — integrate real-time public data sources into applications using AI-assisted discovery


## Available Tools
- **get_dataset**: Get details for a specific dataset
- **get_most_recent_datasets**: Get the most recently added datasets
- **get_most_viewed_datasets**: Get the most viewed datasets
- **list_datasets**: List all datasets in the catalog
- **list_groups**: List all groups in the catalog
- **list_organizations**: List all organizations in the catalog
- **search_datasets**: Search for datasets in the catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Región de Murcia Datos Abiertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets about 'medio ambiente' in the Murcia portal."

**🤖 AI Agent:**
> I found several datasets related to the environment. Notable ones include 'Calidad del aire' and 'Espacios naturales protegidos'. Would you like the details for any of these?

---

**👤 You:**
> "Show me the 10 most viewed datasets in Murcia."

**🤖 AI Agent:**
> The most viewed datasets include the 'Directorio de Centros Educativos', 'Presupuestos Municipales', and 'Evolución de la población'. I can fetch the full metadata for any of these if you provide the name.

---

**👤 You:**
> "List all organizations that publish data on the portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are many contributors, including 'Consejería de Salud', 'Ayuntamiento de Murcia', and 'Servicio Murciano de Salud'. Which organization's data are you interested in?


## Installation & Usage

To install and use the **Región de Murcia Datos Abiertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/region-de-murcia-datos-abiertos](https://vinkius.com/mcp/region-de-murcia-datos-abiertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
