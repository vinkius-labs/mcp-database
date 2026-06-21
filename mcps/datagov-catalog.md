# Data.gov Catalog MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datagov-catalog)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/datagov-catalog-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/datagov-catalog-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access the official US Government open data catalog. Search thousands of datasets, organizations, and spatial data directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data.gov Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for NASA datasets related to climate change."

**🤖 AI Agent:**
> I found several NASA datasets. Notable results include 'Global Surface Temperature Analysis' and 'Climate Model Outputs'. Would you like the full metadata for any of these?

---

**👤 You:**
> "List all government organizations that publish data here."

**🤖 AI Agent:**
> I've retrieved the list of publishing organizations. There are over 1,200 entities, including major agencies like NOAA, NASA, and the Department of Education. Which one would you like to explore?

---

**👤 You:**
> "Get the GeoJSON boundary for 'Los Angeles' to filter my search."

**🤖 AI Agent:**
> I've found the location ID for Los Angeles. Retrieving the GeoJSON geometry now... Done. You can now use this boundary to filter datasets using the `search_datasets` tool.


## Installation & Usage

To install and use the **Data.gov Catalog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datagov-catalog](https://vinkius.com/mcp/datagov-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
