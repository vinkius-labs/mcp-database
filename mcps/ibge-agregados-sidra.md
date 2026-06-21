# IBGE Agregados (SIDRA) MCP Server

Access official Brazilian statistical data from IBGE SIDRA — query surveys, metadata, variables, and geographic levels directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ibge-agregados-sidra)

## Overview
**Category:** data-analytics
**Tools Count:** 5

## Description
Connect to the **IBGE SIDRA** (System for Automatic Recovery) database and explore Brazil's official statistical aggregates through natural language. This server provides a direct interface to the most comprehensive source of Brazilian demographic and economic data.

### What you can do

- **Survey Discovery** — List and filter IBGE aggregates (tables) by subject, period, or classification to find exactly the data you need.
- **Metadata Inspection** — Retrieve detailed metadata for specific tables to understand the context and methodology of the data.
- **Variable Analysis** — Identify all available variables within an aggregate to prepare precise data queries.
- **Temporal Coverage** — Check available time periods for any survey to build historical series or snapshots.
- **Geographic Granularity** — Discover which territorial levels (National, State, City, etc.) are available for specific datasets.

### How it works

1. Subscribe to this server
2. No complex API keys are required for this public data service
3. Start querying Brazilian statistics directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Analysts** — quickly locate specific tables and variables for economic or social modeling.
- **Researchers & Academics** — access official census and survey metadata without navigating complex web portals.
- **Developers** — integrate official Brazilian statistics into applications with ease.


## Available Tools
- **get_localidades**: Get available geographic levels for an aggregate
- **get_metadados**: Get metadata for a specific aggregate
- **get_periodos**: Get available time periods for an aggregate
- **get_variaveis**: Get variables for a specific aggregate
- **list_agregados**: Allows multidimensional filtering.

List IBGE aggregates (surveys/tables)


## Installation & Usage

To install and use the **IBGE Agregados (SIDRA)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ibge-agregados-sidra](https://vinkius.com/mcp/ibge-agregados-sidra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
