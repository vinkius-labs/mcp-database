# Comunidad de Madrid (Portal Regional) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/comunidad-de-madrid-portal-regional)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/comunidad-de-madrid-portal-regional-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/comunidad-de-madrid-portal-regional-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the official Open Data portal of the Community of Madrid. Search datasets, inspect public resources, and query the datastore for regional information.

## Description
Connect your AI agent to the **Comunidad de Madrid Open Data Portal** to access a wealth of public information directly through natural language. This MCP server provides a bridge to the regional CKAN-based repository, covering everything from transport and health to environment and economy.

### What you can do

- **Dataset Discovery** — Search for specific datasets using keywords like 'transporte', 'salud', or 'medio ambiente' to find relevant public records.
- **Metadata Inspection** — Retrieve full metadata for datasets, including tags, organizations, and update frequencies.
- **Resource Management** — List and inspect individual files (resources) within a dataset, such as CSVs, JSONs, or PDFs.
- **Direct Data Querying** — Use the DataStore integration to query the actual content of datasets directly, allowing for data analysis without manual downloads.
- **Portal Exploration** — List all available dataset identifiers to understand the scope of available regional data.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Comunidad de Madrid CKAN API Key for higher rate limits
3. Start querying regional data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly pull regional statistics and records into your workflow for analysis.
- **Developers** — integrate real-time public data from Madrid into applications without navigating complex API docs.
- **Researchers & Citizens** — find public information about air quality, transport schedules, or economic indicators through simple conversation.


## Available Tools
- **get_dataset**: Get full metadata for a specific dataset
- **get_resource**: Get metadata for a specific resource
- **list_datasets**: List all dataset identifiers in the portal
- **search_datasets**: g., transporte, salud).

Search for datasets matching specific criteria
- **search_datastore**: Query data directly from a resource in the DataStore


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Comunidad de Madrid (Portal Regional)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to air quality in Madrid."

**🤖 AI Agent:**
> I found several datasets. The most relevant is 'Calidad del aire: datos diarios' (ID: calidad_aire_datos_dia). Would you like to see its metadata or available resources?

---

**👤 You:**
> "List all dataset identifiers available in the portal."

**🤖 AI Agent:**
> Fetching the list of datasets... There are over 500 datasets available. Some examples include 'centros_salud', 'transporte_publico_lineas', and 'presupuestos_municipales'.

---

**👤 You:**
> "Get the metadata for the dataset 'calidad_aire_datos_dia'."

**🤖 AI Agent:**
> The dataset 'Calidad del aire: datos diarios' is managed by the Environment department. It contains 12 resources (CSV and Excel files) and is updated daily. Would you like the ID of the latest CSV resource?


## Installation & Usage

To install and use the **Comunidad de Madrid (Portal Regional)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/comunidad-de-madrid-portal-regional](https://vinkius.com/mcp/comunidad-de-madrid-portal-regional)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
