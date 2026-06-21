# Gipuzkoa Irekia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gipuzkoa-irekia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gipuzkoa-irekia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gipuzkoa-irekia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access open data from Gipuzkoa (Spain) — search datasets, explore resources, and query organizations or thematic groups directly from any AI agent.

## Description
Connect to the **Gipuzkoa Irekia** open data portal and empower your AI agent to explore public sector information from the Gipuzkoa region through natural conversation.

### What you can do

- **Dataset Discovery** — Search for specific datasets (packages) using keywords or filter by organization and metadata
- **Resource Inspection** — Access detailed metadata for specific data files (resources), including formats and download links
- **Organizational Browsing** — List and inspect the various public departments and municipalities that publish data
- **Thematic Exploration** — Navigate data through thematic groups such as transport, environment, or economy
- **Advanced Querying** — Perform Solr-like searches to find precise information within the vast public catalog

### How it works

1. Subscribe to this server
2. Enter your Gipuzkoa Irekia API Key (optional for public data, recommended for higher limits)
3. Start querying public datasets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and inspect public datasets for research and reporting without manual portal navigation
- **Developers** — retrieve resource IDs and metadata directly in the IDE to integrate public APIs into applications
- **Citizens & Researchers** — explore government transparency data and public records through simple natural language questions


## Available Tools
- **list_groups**: List all group names
- **show_group**: Get details for a specific group
- **list_organizations**: List all organization names
- **show_organization**: Get details for a specific organization
- **list_packages**: List all dataset (package) names
- **search_packages**: Search for datasets
- **show_package**: Get metadata for a specific dataset
- **search_resources**: Search for resources
- **show_resource**: Get metadata for a specific resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gipuzkoa Irekia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the organizations that publish open data in Gipuzkoa."

**🤖 AI Agent:**
> I've retrieved the list of publishing organizations. There are several entities including 'Diputación Foral de Gipuzkoa', 'Ayuntamiento de Donostia', and various regional agencies. Would you like to see the details for a specific one?

---

**👤 You:**
> "Search for datasets related to 'environment' in the Gipuzkoa Irekia catalog."

**🤖 AI Agent:**
> Searching for 'environment'... I found several datasets, such as 'Air Quality Measurements' and 'Waste Management Statistics'. Which one would you like to explore further?

---

**👤 You:**
> "Show me the metadata for the dataset named 'presupuestos-municipales'."

**🤖 AI Agent:**
> Fetching metadata for 'presupuestos-municipales'... This dataset contains municipal budget information. It includes resources in CSV and XLS formats, last updated recently by the Finance Department. Do you want the specific resource IDs for downloading?


## Installation & Usage

To install and use the **Gipuzkoa Irekia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gipuzkoa-irekia](https://vinkius.com/mcp/gipuzkoa-irekia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
