# CNMC (Comisión Mercados y Competencia) MCP Server

Access Spanish market and competition data — search datasets and retrieve records from the CNMC open data portal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia)

## Overview
**Category:** data-analytics
**Tools Count:** 2

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


## Installation & Usage

To install and use the **CNMC (Comisión Mercados y Competencia)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia](https://vinkius.com/mcp/cnmc-comision-mercados-y-competencia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
