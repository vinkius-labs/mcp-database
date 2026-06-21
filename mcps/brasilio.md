# Brasil.io MCP Server

Access structured Brazilian public data — query COVID-19 stats, company records, and socio-economic datasets directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/brasilio)

## Overview
**Category:** data-analytics
**Tools Count:** 3

## Description
Connect to **Brasil.io**, the leading platform for accessible Brazilian public data, and empower your AI agent to analyze real-world datasets through natural conversation.

### What you can do

- **Dataset Discovery** — List all available public datasets hosted on the platform, from health data to judicial salaries.
- **Metadata Inspection** — Fetch detailed schemas and metadata for specific tables to understand available columns and data types.
- **Advanced Querying** — Retrieve actual data records with powerful filtering capabilities (by state, city, date, etc.) using simple JSON filters.
- **Pagination Support** — Navigate through large datasets efficiently using built-in pagination controls.

### How it works

1. Subscribe to this server
2. Enter your Brasil.io API Token
3. Start querying Brazilian public intelligence from Claude, Cursor, or any MCP client

No more manual CSV downloads or wrestling with government transparency portals. Your AI acts as a data scientist specialized in Brazilian public records.

### Who is this for?

- **Data Analysts & Journalists** — quickly extract facts and figures for reports without writing complex scrapers.
- **Researchers** — access historical and current socio-economic data for academic or market studies.
- **Developers** — integrate real Brazilian administrative data into your workflows or applications via your IDE.


## Available Tools
- **list_datasets**: io platform. Supports pagination.

List available datasets on Brasil.io
- **query_table_data**: You can pass arbitrary filters as a JSON string to filter by column names (e.g., {"state": "PR"}).

Query data records from a specific table
- **get_table_metadata**: Get metadata for a specific table in a dataset


## Installation & Usage

To install and use the **Brasil.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brasilio](https://vinkius.com/mcp/brasilio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
