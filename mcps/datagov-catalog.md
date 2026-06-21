# Data.gov Catalog MCP Server

Access the official US Government open data catalog. Search thousands of datasets, organizations, and spatial data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datagov-catalog)

## Overview
**Category:** data-analytics
**Tools Count:** 8

## Description
Connect to the **Data.gov Catalog** to explore the comprehensive repository of US Government open data. This MCP server allows AI agents to discover datasets from agencies like NASA, NOAA, and the Census Bureau through natural language.

### What you can do

- **Dataset Discovery** — Search the entire catalog using keywords, organization filters, and advanced sorting via `search_datasets`.
- **Spatial Analysis** — Find datasets by geographic location using GeoJSON boundaries and spatial filters with `search_locations` and `get_location_geometry`.
- **Organization Insights** — List all publishing organizations and filter results by specific agency slugs using `get_organizations`.
- **Metadata Inspection** — Retrieve detailed harvest records, including raw and transformed DCAT-US payloads with `get_harvest_record_raw` and `get_harvest_record_transformed`.
- **Keyword Trends** — Analyze commonly used keywords and their dataset counts to identify data trends using `get_keywords`.

### How it works

1. Subscribe to this server
2. Enter 'PUBLIC' or your API key if required by your proxy
3. Start querying the US Government's open data repository directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists** — quickly find relevant datasets for analysis without manual browsing
- **Researchers** — access official government metadata and harvest records for academic or policy work
- **Developers** — integrate public data sources into applications using structured GeoJSON and DCAT-US metadata


## Available Tools
- **get_location_geometry**: Retrieve the GeoJSON boundary for a specific location ID
- **get_harvest_record_raw**: Retrieve original unmodified source payload for a harvest record
- **get_harvest_record**: Retrieve metadata about how a dataset was ingested
- **get_harvest_record_transformed**: Retrieve transformed DCAT-US payload for a harvest record
- **get_keywords**: Retrieve commonly used keywords and their dataset counts
- **get_organizations**: Retrieve the complete list of publishing organizations
- **search_locations**: Autocomplete search for location names to use with spatial filtering
- **search_datasets**: Search the catalog using keywords, filters, and sorting


## Installation & Usage

To install and use the **Data.gov Catalog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datagov-catalog](https://vinkius.com/mcp/datagov-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
