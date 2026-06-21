# CNMC (Comisión Mercados y Competencia) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cnmc-comision-mercados-y-competencia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cnmc-comision-mercados-y-competencia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Spanish market and competition data — search datasets and retrieve records from the CNMC open data portal.

## Description
Connect to the official Open Data portal of the **CNMC (Comisión Nacional de los Mercados y la Competencia)**. This server allows AI agents to explore and extract public data regarding telecommunications, energy, transport, and postal sectors in Spain.

### What you can do

- **Catalog Discovery** — Use `package_search` to find datasets, resources, and metadata using keywords or specific queries.
- **Data Extraction** — Use `datastore_search` to pull actual records and rows from specific resources using their unique IDs.
- **Granular Filtering** — Apply JSON filters to narrow down results to specific dates, regions, or categories within a dataset.
- **Resource Inspection** — Identify update frequencies, license types, and resource formats before processing data.

### How it works

1. Subscribe to this server
2. Enter your CNMC API Key (if required for higher rate limits)
3. Start querying Spanish market data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly fetch market statistics without manual CSV downloads
- **Legal & Compliance Teams** — monitor regulatory data and competition records
- **Policy Researchers** — access public sector information for economic modeling and reporting


## Available Tools
- **datastore_search**: g., a CSV file within a dataset). Requires a resource_id obtained via package_search.

Retrieve actual records from a specific CNMC resource
- **package_search**: Use this to find the resource_id needed for datastore_search.

Search for datasets and resources in the CNMC catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CNMC (Comisión Mercados y Competencia)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets related to 'energía eléctrica' in the CNMC catalog."

**🤖 AI Agent:**
> I found several datasets. The most relevant one is 'Estadística mensual de energía eléctrica' with resource ID 'e123-abc'. Would you like me to fetch the latest records from it?

---

**👤 You:**
> "Get the first 5 records from the CNMC resource '06935639-5561-4608-9580-59367208479e'."

**🤖 AI Agent:**
> I've retrieved the first 5 records for that resource. They include data on market shares for telecommunications operators in Q1 2023. [Data table displayed...]

---

**👤 You:**
> "Search for 'gas natural' datasets and filter the results for the year 2022."

**🤖 AI Agent:**
> I've identified the 'Consumo de gas natural' dataset. Applying the filter for 2022... I found 12 monthly records. Would you like a summary of the total consumption?


## Installation & Usage

To install and use the **CNMC (Comisión Mercados y Competencia)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia](https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
