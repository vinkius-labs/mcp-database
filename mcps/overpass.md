# Overpass MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/overpass)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/overpass-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/overpass-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access OpenStreetMap data via Overpass API — execute complex spatial queries, fetch raw map data, and monitor API status.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Overpass** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Use execute_query to find all hospitals within 5km of coordinates 51.5074, -0.1278."

**🤖 AI Agent:**
> I've executed the Overpass query. I found 12 hospitals in that radius, including St Thomas' Hospital and Guy's Hospital. Would you like the specific coordinates for any of them?

---

**👤 You:**
> "Get the raw OSM map data for the area 13.3,52.5,13.4,52.6 using get_map."

**🤖 AI Agent:**
> I have retrieved the raw XML map data for that bounding box. It contains all nodes, ways, and relations within those coordinates. How would you like me to process this data?

---

**👤 You:**
> "Check my current Overpass API status and rate limits."

**🤖 AI Agent:**
> Checking status... You currently have 2 slots available, and no active rate limit cooldowns. You are free to execute more queries.


## Installation & Usage

To install and use the **Overpass** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/overpass](https://vinkius.com/mcp/overpass)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
