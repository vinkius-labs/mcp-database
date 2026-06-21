# Overpass MCP Server

Access OpenStreetMap data via Overpass API — execute complex spatial queries, fetch raw map data, and monitor API status.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/overpass)

## Overview
**Category:** data-analytics
**Tools Count:** 4

## Description
Connect your AI agent to the **Overpass API** to query and retrieve OpenStreetMap (OSM) data globally. This server allows for deep geospatial analysis and data extraction through natural language.

### What you can do

- **Advanced Spatial Queries** — Use `execute_query` with Overpass QL to find specific points of interest (POIs), ways, or relations (e.g., all pharmacies in a city).
- **Map Data Extraction** — Use `get_map` to fetch raw OSM XML data for a specific bounding box for GIS processing.
- **Legacy Support** — Execute queries using the `execute_xapi` tool for compatibility with legacy XAPI syntax.
- **Rate Limit Management** — Use `get_status` to check your current API slot availability and avoid being throttled during heavy data collection.

### How it works

1. Subscribe to this server
2. (Optional) Configure your preferred Overpass instance URL
3. Start asking your AI to find locations, analyze urban infrastructure, or download map segments

### Who is this for?

- **Data Scientists & GIS Analysts** — automate the extraction of geographic features for research and modeling.
- **Urban Planners** — quickly query city infrastructure like bike lanes, parks, or public transport nodes.
- **Developers** — integrate real-world map data into applications without manually writing complex API calls.


## Available Tools
- **execute_query**: ALWAYS include [out:json]; at the beginning of your query to ensure JSON output.

Execute an Overpass QL query
- **get_map**: Returns raw XML data.

Fetch OSM map data for a bounding box
- **get_status**: Check Overpass API rate limit and slot status
- **execute_xapi**: Returns raw XML data.

Execute a legacy XAPI query


## Installation & Usage

To install and use the **Overpass** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/overpass](https://vinkius.com/mcp/overpass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
