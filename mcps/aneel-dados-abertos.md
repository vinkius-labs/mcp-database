# ANEEL Dados Abertos MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aneel-dados-abertos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aneel-dados-abertos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aneel-dados-abertos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the Brazilian National Electric Energy Agency (ANEEL) Open Data Portal to query electricity sector datasets, resources, and records.

## Description
Connect your AI agent to the **ANEEL Open Data Portal** (Agência Nacional de Energia Elétrica) and explore comprehensive information about the Brazilian electricity market through natural conversation.

### What you can do

- **Dataset Discovery** — List all available packages (datasets) in the portal to understand what information is public.
- **Metadata Inspection** — Fetch detailed metadata for specific datasets, including tags, organizations, and available resources.
- **Resource Details** — Get specific information about files (CSV, PDF, XLS), including download URLs and formats.
- **Deep Data Search** — Query and filter records directly within CSV/XLS resources that are integrated into the ANEEL DataStore API.

### How it works

1. Subscribe to this server
2. (Optional) Enter your ANEEL API Key if you have specific access requirements
3. Start querying energy data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly find and filter energy tariffs, generation data, and distribution metrics.
- **Energy Consultants** — retrieve regulatory data and infrastructure information without manual portal navigation.
- **Developers** — integrate public energy data into applications using structured queries via the AI agent.


## Available Tools
- **get_package**: Get full metadata for a specific ANEEL dataset
- **get_resource**: g., CSV, PDF file) within a dataset, including its download URL and format.

Get metadata for a specific ANEEL resource
- **list_packages**: List all dataset names in the ANEEL portal
- **search_datastore**: Search for records within an ANEEL resource


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ANEEL Dados Abertos** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available datasets in the ANEEL portal."

**🤖 AI Agent:**
> I've retrieved the list of packages. There are several datasets available, including 'tarifas-distribuidoras', 'geracao-distribuida', and 'interrupcoes-energia'. Which one would you like to explore?

---

**👤 You:**
> "Show me the resources available for the 'tarifas-distribuidoras' package."

**🤖 AI Agent:**
> The 'tarifas-distribuidoras' package contains 3 resources: a CSV file with current rates (ID: res-123), a PDF manual (ID: res-456), and a historical XLS file (ID: res-789).

---

**👤 You:**
> "Search for records related to 'ENEL' in the resource with ID 'd345-f678'."

**🤖 AI Agent:**
> Searching the datastore... I found 15 records for 'ENEL' in that resource. The most recent entries show tariff adjustments and operational metrics for the São Paulo region.


## Installation & Usage

To install and use the **ANEEL Dados Abertos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aneel-dados-abertos](https://vinkius.com/mcp/aneel-dados-abertos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
