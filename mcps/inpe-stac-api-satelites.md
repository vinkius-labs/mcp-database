# INPE (STAC API - Satélites) MCP Server

Access Brazil's National Institute for Space Research (INPE) satellite data via STAC API — search collections, list items, and query Earth observation metadata.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/inpe-stac-api-satelites)

## Overview
**Category:** government-public-data
**Tools Count:** 6

## Description
Connect to the **INPE Brazil Data Cube** and explore high-resolution satellite imagery catalogs through natural language. This server implements the STAC (SpatioTemporal Asset Catalog) specification to provide seamless access to Earth observation data from missions like CBERS, Sentinel, and Landsat.

### What you can do

- **Catalog Discovery** — Explore the root catalog and check conformance classes of the INPE STAC server using `get_root_catalog` and `get_conformance`.
- **Collection Browsing** — List all available data collections (e.g., CBERS4, Sentinel-2) and fetch detailed metadata for specific ones with `list_collections` and `get_collection`.
- **Item Listing** — Retrieve specific scenes and assets within a collection using spatial (bounding box) and temporal filters via `list_collection_items`.
- **Advanced Search** — Perform cross-collection searches to find the exact satellite imagery needed for environmental monitoring or research using `search_items`.

### How it works

1. Subscribe to this server
2. Enter your Brazil Data Cube (BDC) Access Key
3. Start querying satellite metadata from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — Quickly find satellite scenes for specific dates and regions without manual API calls or complex scripts.
- **Environmental Analysts** — Monitor land use, deforestation, or agricultural changes using INPE's curated data cubes directly from your AI assistant.
- **GIS Developers** — Integrate satellite metadata discovery and asset retrieval directly into your development workflow.


## Available Tools
- **list_collection_items**: List items within a specific collection
- **get_collection**: Get detailed metadata for a specific collection
- **list_collections**: g., CBERS4-WFI-16D-2, S2-16D-2).

List all available data collections
- **get_conformance**: Get STAC conformance classes
- **get_root_catalog**: Get the root STAC catalog
- **search_items**: Search for items across collections


## Installation & Usage

To install and use the **INPE (STAC API - Satélites)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inpe-stac-api-satelites](https://vinkius.com/mcp/inpe-stac-api-satelites)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
