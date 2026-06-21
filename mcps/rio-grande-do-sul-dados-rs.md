# Rio Grande do Sul (Dados RS) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rio-grande-do-sul-dados-rs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rio-grande-do-sul-dados-rs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rio-grande-do-sul-dados-rs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access the official Open Data portal of Rio Grande do Sul — query public datasets, government organizations, and thematic groups directly.

## Description
Connect to the **Dados RS** portal and explore the public data infrastructure of Rio Grande do Sul, Brazil. This server allows any AI agent to interact with the state's CKAN-based repository to find, inspect, and analyze government information.

### What you can do

- **Dataset Discovery** — List all available datasets or search for specific topics like health, education, or finance using keywords.
- **Organization Insights** — Explore the government bodies (organizations) that publish data and list their specific contributions.
- **Thematic Browsing** — Navigate data through thematic groups such as 'Environment', 'Security', or 'Economy'.
- **Deep Data Querying** — Access tabular data within resources using filters or execute complex SQL queries directly against the DataStore.
- **Resource Inspection** — Fetch metadata for specific files, links, and data distributions to understand their structure before downloading.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Dados RS API Key for higher rate limits
3. Start querying public data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — quickly find and query government statistics without manual CSV downloads
- **Journalists** — audit public spending and government actions through direct access to official records
- **Developers** — integrate real-time public data into applications using the DataStore SQL capabilities


## Available Tools
- **search_datastore_sql**: SQL Query on DataStore
- **search_datastore**: Search DataStore
- **list_groups**: List groups
- **show_group**: Show group details
- **list_organizations**: List organizations
- **show_organization**: Show organization details
- **list_datasets**: List all datasets (packages)
- **search_datasets**: Search datasets (packages)
- **show_dataset**: Show dataset details
- **search_resources**: Search resources
- **show_resource**: Show resource details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rio Grande do Sul (Dados RS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets about 'educação' in Rio Grande do Sul."

**🤖 AI Agent:**
> I found several datasets related to education, including 'Escolas Estaduais' and 'Taxa de Analfabetismo'. Which one would you like to explore further?

---

**👤 You:**
> "List all government organizations available on the Dados RS portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are over 50 bodies, including the 'Secretaria da Saúde', 'Secretaria da Fazenda', and 'Brigada Militar'.

---

**👤 You:**
> "Show the details for the dataset 'receita-corrente-liquida'."

**🤖 AI Agent:**
> The dataset 'Receita Corrente Líquida' contains metadata about state revenue. It includes 3 resources (CSV and PDF) and is maintained by the Secretaria da Fazenda.


## Installation & Usage

To install and use the **Rio Grande do Sul (Dados RS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rio-grande-do-sul-dados-rs](https://vinkius.com/mcp/rio-grande-do-sul-dados-rs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
