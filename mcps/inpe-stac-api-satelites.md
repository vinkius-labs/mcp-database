# INPE (STAC API - Satélites) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inpe-stac-api-satelites)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/inpe-stac-api-satelites-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/inpe-stac-api-satelites-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access Brazil's National Institute for Space Research (INPE) satellite data via STAC API — search collections, list items, and query Earth observation metadata.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **INPE (STAC API - Satélites)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available satellite data collections from INPE."

**🤖 AI Agent:**
> I've retrieved the available collections from the INPE STAC server. You can access datasets such as 'CBERS4-WFI-16D-2', 'S2-16D-2', and 'LANDSAT-8-16D-2'. Which one would you like to explore further?

---

**👤 You:**
> "Search for satellite items in the bounding box [-48, -16, -47, -15] for the year 2023."

**🤖 AI Agent:**
> Searching across collections... I found several items matching your criteria. For example, in the 'S2-16D-2' collection, there are scenes from various dates in 2023 covering those coordinates. Would you like the specific asset links for one of these items?

---

**👤 You:**
> "Get details for the collection 'CBERS4-WFI-16D-2'."

**🤖 AI Agent:**
> The 'CBERS4-WFI-16D-2' collection is a 16-day surface reflectance composite from the CBERS-4 WFI sensor. It covers the period from 2014 to the present and includes bands like Blue, Green, Red, and NIR. Do you want to list the most recent items from this collection?


## Installation & Usage

To install and use the **INPE (STAC API - Satélites)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inpe-stac-api-satelites](https://vinkius.com/mcp/inpe-stac-api-satelites)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
