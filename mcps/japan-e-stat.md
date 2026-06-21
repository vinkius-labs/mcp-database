# Japan e-Stat MCP Server

Query official Japanese government statistics — population, GDP, industry, trade, employment, and more — from the e-Stat national database.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/japan-e-stat)

## Overview
**Category:** data-analytics
**Tools Count:** 2

## Description
The **Japan e-Stat MCP Server** connects your AI agent to the official Portal of Government Statistics of Japan — the most comprehensive public data repository for the world's third-largest economy.

### Core Capabilities

- **Table Search** — Discover statistical tables across all Japanese government ministries by keyword. Covers census data, national accounts, industrial production, foreign trade, labor force surveys, and more.
- **Data Retrieval** — Pull raw numerical data from any table, fully classified by category, geographic area, and time period.
- **English Support** — The API supports `lang=E` for English-translated table names and categories where available.

Free API key required (instant registration at e-stat.go.jp). Japan publishes some of the most detailed and reliable economic statistics in the world, making this an essential resource for global macro analysis, trade research, and market intelligence.


## Available Tools
- **get_japan_stats_data**: Use search_japan_statistics first to find the correct table ID. Returns category-classified data with time periods, areas, and values.

Retrieve statistical data from a specific Japanese Government e-Stat table
- **search_japan_statistics**: Returns table IDs, organization names, titles, and survey dates. Use the returned table ID with get_japan_stats_data to retrieve actual numbers. Keywords work in both English and Japanese. Common topics: population, GDP, industry, trade, employment, tourism, education, health.

Search for statistical tables in the Japanese Government e-Stat database


## Installation & Usage

To install and use the **Japan e-Stat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/japan-e-stat](https://vinkius.com/mcp/japan-e-stat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
