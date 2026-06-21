# FRED Tags & Sources — Data Discovery MCP Server

Discover FRED series through intelligent tagging: search tags like 'gdp', 'inflation', 'monthly', combine multiple tags to find exactly the right series, and explore all 107 official data sources from BLS to the Census Bureau.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-tags-sources-data-discovery)

## Overview
**Category:** brain-trust
**Tools Count:** 3

## Description
The discovery layer for FRED. Tags & Sources helps your AI agent find exactly the right series by filtering through FRED's comprehensive tagging system.

### What you can do
- **Search Tags** — Browse geographic (usa, europe), topic (gdp, inflation), source (bls, bea), and frequency (monthly, quarterly) tags
- **Tag Combinations** — Find series matching ALL specified tags (e.g., usa + gdp + quarterly) while excluding others
- **Data Sources** — List all 107 organizations contributing data: BLS, BEA, Federal Reserve Board, Census Bureau, Treasury, IMF, and more

### Who is this for?
Researchers exploring FRED's catalog, data engineers building automated pipelines, and AI agents that need precise series discovery beyond simple keyword search.


## Available Tools
- **search_tags**: Search by text or get all tags. Tags include geographic (usa, europe), topic (gdp, inflation), source (bls, bea), and frequency (monthly, quarterly) labels.

Search or browse FRED tags
- **get_series_by_tags**: Powerful for discovering related series. Example: tag_names="usa;gdp" returns all US GDP series. Combine with exclude_tag_names to refine.

Get FRED series matching specific tags
- **list_sources**: List all FRED data sources


## Installation & Usage

To install and use the **FRED Tags & Sources — Data Discovery** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-tags-sources-data-discovery](https://vinkius.com/mcp/fred-tags-sources-data-discovery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
