# USITC DataWeb (International Trade Commission) MCP Server

Access US international trade statistics directly. Query imports, exports, and trade balances using HS, SITC, or NAICS classifications.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/usitc-dataweb-international-trade-commission)

## Overview
**Category:** industry-titans
**Tools Count:** 4

## Description
Connect to the **USITC DataWeb** to retrieve official US international trade data. This server allows AI agents to perform complex queries on trade statistics, including imports, exports, and trade balances across various classification systems like HS, SITC, and NAICS.

### What you can do

- **Trade Data Queries** — Fetch detailed statistics by commodity, country, and time period using the `query_trade_data` tool.
- **Metadata Exploration** — List available data tables, fields, and valid values (like country codes or commodity levels) to build precise queries.
- **Classification Support** — Work with Harmonized Tariff Schedule (HS), SITC, or NAICS codes at various digit levels.
- **Time-Series Analysis** — Retrieve annual or monthly data to analyze trade trends over time.

### How it works

1. Subscribe to this server
2. Enter your USITC DataWeb API Key
3. Start analyzing global trade patterns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Economists & Analysts** — instantly retrieve trade volumes and values for specific sectors without manual CSV downloads.
- **Supply Chain Managers** — monitor international trade flows and commodity trends directly from your workspace.
- **Policy Researchers** — audit trade balances and historical data using official government sources.


## Available Tools
- **list_metadata_fields**: List fields available for a specific table
- **list_metadata_tables**: List available data tables
- **list_metadata_values**: g., a list of all valid country codes).

List valid values for a specific field within a table
- **query_trade_data**: Uses POST to support large filter sets.

Query USITC trade statistics


## Installation & Usage

To install and use the **USITC DataWeb (International Trade Commission)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/usitc-dataweb-international-trade-commission](https://vinkius.com/mcp/usitc-dataweb-international-trade-commission)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
