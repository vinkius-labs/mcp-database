# São Paulo (Cidade) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sao-paulo-cidade)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sao-paulo-cidade-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sao-paulo-cidade-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the official São Paulo Open Data portal — search datasets, query resources via SQL, and explore city organizations and themes.

## Description
Connect your AI agent directly to the **São Paulo City Open Data Portal (CKAN)**. This server allows you to navigate thousands of public datasets covering health, education, transport, and finance in Brazil's largest city.

### What you can do

- **Dataset Discovery** — Search for specific datasets using keywords or list all available packages in the portal.
- **Granular Inspection** — Fetch detailed metadata for datasets and individual resources (files) to understand data structures.
- **Advanced Data Querying** — Perform searches within data stores or execute complex SQL queries directly on CSV-backed resources.
- **Organizational Mapping** — List and inspect city secretariats (organizations) and thematic groups to find relevant data sources.
- **Tag Exploration** — Browse datasets by tags to discover related public information across different departments.

### How it works

1. Subscribe to this server
2. (Optional) Provide your São Paulo Open Data API Key for higher rate limits
3. Start querying city data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts & Researchers** — quickly find and query public statistics without manual downloads
- **Developers** — integrate real-time city data into applications using SQL-like queries
- **Journalists & Citizens** — audit public spending and city performance through natural language conversation


## Available Tools
- **datastore_search_sql**: SQL Query on a resource
- **datastore_search**: Search data within a resource
- **list_groups**: g., Educação, Meio Ambiente).

List groups (themes)
- **get_group**: Get group details
- **list_organizations**: g., Secretarias) that own datasets.

List organizations
- **get_organization**: Get organization details
- **list_packages**: List all datasets (packages) in the portal
- **search_packages**: Search datasets
- **get_package**: Get dataset details
- **get_resource**: Get resource details
- **list_tags**: List tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **São Paulo (Cidade)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets about public transport in São Paulo."

**🤖 AI Agent:**
> I found several datasets related to public transport. The most relevant are 'Bilhete Único statistics' and 'Bus lines and stops'. Would you like to see the resources for one of these?

---

**👤 You:**
> "List all organizations that provide open data in the portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are over 50 entities, including 'Secretaria Municipal da Saúde', 'Secretaria Municipal de Educação', and 'SPTrans'. Which one should we explore?

---

**👤 You:**
> "Get the details for the dataset 'folha-de-pagamento'."

**🤖 AI Agent:**
> The dataset 'folha-de-pagamento' contains payroll information for city employees. It has 12 resources available, mostly in CSV and PDF formats. Would you like the ID of the latest CSV resource to query it?


## Installation & Usage

To install and use the **São Paulo (Cidade)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sao-paulo-cidade](https://vinkius.com/mcp/sao-paulo-cidade)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
