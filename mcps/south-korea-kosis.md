# South Korea KOSIS MCP Server

Query official South Korean government statistics — demographics, GDP, trade, technology, and industry — from the KOSIS national database.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/south-korea-kosis)

## Overview
**Category:** data-analytics
**Tools Count:** 2

## Description
The **South Korea KOSIS MCP Server** connects your AI agent to the Korean Statistical Information Service — the official data portal for the world's 12th-largest economy and a global powerhouse in semiconductors, automotive, and electronics.

### Core Capabilities

- **Table Search** — Discover statistical tables across all Korean government agencies by keyword. Covers the full spectrum from demographics and national accounts to semiconductor production and trade flows.
- **Data Retrieval** — Pull raw numerical data from any KOSIS table, organized by classification and time period with full unit annotations.
- **Period Filtering** — Narrow results to specific time ranges using start/end period parameters.

Free API key required (instant registration at kosis.kr). South Korea publishes highly granular data covering semiconductor exports, technology adoption, and manufacturing output — intelligence that is critical for supply chain analysis and technology market research.


## Available Tools
- **get_korea_stats_data**: Requires orgId and tableId from search_korea_statistics. Optionally filter by time period (YYYYMM or YYYY format).

Retrieve statistical data from a specific KOSIS table in South Korea
- **search_korea_statistics**: Returns table IDs, organization IDs, and table names. Use returned orgId and tableId with get_korea_stats_data to retrieve numbers. Common topics: population, GDP, semiconductor exports, technology, employment, trade, education, housing.

Search for statistical tables in the South Korean KOSIS national database


## Installation & Usage

To install and use the **South Korea KOSIS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/south-korea-kosis](https://vinkius.com/mcp/south-korea-kosis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
