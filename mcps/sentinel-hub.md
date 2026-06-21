# Sentinel Hub MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sentinel-hub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sentinel-hub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sentinel-hub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Access and process satellite imagery from Sentinel, Landsat, and other Earth observation missions through a powerful cloud API.

## Description
Connect to **Sentinel Hub** — the most powerful satellite imagery processing API in Europe — and transform raw Earth observation data into actionable intelligence.

### What you can do

- **STAC Catalog Search** — Discover available satellite scenes by location, date, collection, cloud cover, and MGRS tile ID across all Sentinel missions and Landsat
- **Image Processing** — Render custom satellite imagery using evalscripts (JavaScript-based processing scripts) that define how bands are combined, indices are calculated, and pixels are colored
- **Vegetation Analysis (NDVI)** — Generate ready-to-use NDVI evalscripts that color-code vegetation density from bare soil to dense forest
- **Statistical Analysis** — Calculate mean, min, max, standard deviation, and histograms over areas of interest with temporal aggregation (daily, weekly, monthly)
- **Cloud-Free Search** — Find satellite scenes below a specified cloud cover threshold for clean optical analysis
- **Band Combinations** — Access a curated library of 10 predefined band combinations including True Color, False Color, NDWI, Moisture Index, SWIR, and Burn Severity

### How it works

1. Subscribe to this server
2. Register at [dataspace.copernicus.eu](https://dataspace.copernicus.eu/) and create an OAuth2 client
3. Enter your credentials as `client_id:client_secret`
4. Start processing satellite imagery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **GIS Professionals** — process satellite imagery on-demand without downloading terabytes of raw data
- **Environmental Scientists** — compute vegetation, water, and moisture indices for monitoring ecosystems
- **Urban Planners** — analyze land use changes with multi-temporal statistical analysis
- **Agricultural Advisors** — monitor crop health with NDVI time series and cloud-free imagery selection
- **Emergency Managers** — assess wildfire damage with burn severity indices in near real-time


## Available Tools
- **catalog_search**: Specify a collection ID (e.g., "sentinel-2-l2a", "sentinel-1-grd"), a bounding box as [west, south, east, north] coordinates, and a date range. Returns item metadata including geometry, cloud cover, and band information.

Search the Sentinel Hub STAC catalog for satellite imagery
- **check_sentinel_hub_status**: Returns the connection status and service URL. Use this to verify your client_id:client_secret credentials are working correctly.

Verify Sentinel Hub API connectivity and authentication
- **generate_false_color_evalscript**: In the output, healthy vegetation appears bright red, urban areas appear cyan/grey, and water appears dark blue. This is the standard false-color composite used in remote sensing for vegetation mapping and land cover classification.

Generate a false-color evalscript for vegetation emphasis
- **generate_ndvi_evalscript**: The output is color-coded: dark for water/shadow, grey for bare soil, yellow-green for sparse vegetation, and deep green for dense vegetation. Use the returned evalscript with the process_image tool.

Generate a ready-to-use NDVI evalscript for vegetation analysis
- **generate_true_color_evalscript**: Use the returned evalscript with the process_image tool to get visually appealing satellite photos of any location on Earth.

Generate a true-color RGB evalscript for natural imagery
- **get_catalog_collection**: Get detailed information about a specific data collection
- **get_catalog_item**: Use the item ID returned from a catalog_search query.

Get detailed metadata for a specific STAC catalog item
- **get_statistics**: Requires an evalscript that defines which bands to analyze. Supports temporal aggregation (daily, weekly, monthly) for time-series analysis of vegetation indices, water levels, or urban expansion.

Calculate statistics over an area from satellite imagery
- **get_user_info**: Useful for verifying credentials and understanding available quotas.

Get authenticated Sentinel Hub user profile information
- **list_band_combinations**: Includes True Color, False Color (vegetation), NDVI, NDWI, Moisture Index, SWIR, SAR polarizations, Scene Classification, and Burn Severity (NBR). Each entry specifies the required bands and target collection.

List predefined satellite band combinations and indices
- **list_catalog_collections**: Includes Sentinel-1 GRD (radar), Sentinel-2 L1C/L2A (optical), Sentinel-3 OLCI/SLSTR, Sentinel-5P (atmosphere), Landsat 8-9, DEM, and Copernicus Land Monitoring Service data.

List all available Sentinel Hub satellite data collections
- **process_image**: Specify the data collection, area of interest as a bounding box, date range, and the evalscript. The evalscript defines band inputs, processing logic, and output format. Use generate_ndvi_evalscript or generate_true_color_evalscript tools to get ready-made evalscripts.

Process satellite imagery with a custom evalscript
- **search_by_tile**: MGRS tiles are the standard spatial reference for Sentinel-2 data (e.g., "33UUP" for central Europe, "29SQB" for Lisbon area). Returns all scenes for the specified tile within the date range.

Search Sentinel-2 imagery by MGRS tile identifier
- **search_cloud_free**: Essential for optical analysis where cloud contamination would corrupt results. Typical thresholds: <10% for clean analysis, <30% for general use, <50% for temporal coverage.

Search for cloud-free satellite imagery below a threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sentinel Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me an NDVI vegetation analysis for the Amazon rainforest region."

**🤖 AI Agent:**
> I'll start by generating the NDVI evalscript... Done. Now processing Sentinel-2 imagery for the Amazon basin (-65,-5,-55,0) from the last 30 days. The processed result shows a 512x512 pixel NDVI map with dense vegetation (deep green) covering 87% of the area, sparse vegetation (yellow-green) at 8%, and water bodies (dark) at 5%. Would you like time-series statistics to track deforestation trends?

---

**👤 You:**
> "Find cloud-free Sentinel-2 imagery over Paris with less than 10% clouds."

**🤖 AI Agent:**
> Searching for cloud-free scenes over Paris (2.2,48.8,2.5,48.9) with maximum 10% cloud cover... Found 3 scenes from the last month. The cleanest acquisition has 2.1% cloud cover from 5 days ago, captured by Sentinel-2A. The next scene has 7.3% from 10 days ago. Would you like me to generate a true-color image of the cleanest scene?

---

**👤 You:**
> "What band combinations can I use for wildfire assessment?"

**🤖 AI Agent:**
> I've listed the available band combinations. For wildfire assessment, you should use the **Burn Severity (NBR)** index which combines bands B08 (NIR) and B12 (SWIR) from Sentinel-2. For broader context, the **SWIR** composite (B12, B8A, B04) highlights burned areas in distinctive colors. The **False Color (Vegetation)** combination (B08, B04, B03) also clearly distinguishes healthy vegetation from burned areas. Would you like me to process burn severity for a specific region?


## Installation & Usage

To install and use the **Sentinel Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sentinel-hub](https://vinkius.com/mcp/sentinel-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
