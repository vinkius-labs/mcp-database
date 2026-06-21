# Copernicus Data Space MCP Server

Access satellite imagery and Earth observation datasets from the EU Copernicus program for environmental and geospatial analysis.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/copernicus-data-space)

## Overview
**Category:** the-unthinkable
**Tools Count:** 14

## Description
Connect to the **Copernicus Data Space Ecosystem** and unlock the world's largest open Earth observation archive directly from your AI agent.

### What you can do

- **Product Discovery** — Search across Sentinel-1 (radar), Sentinel-2 (optical), Sentinel-3 (ocean/land), Sentinel-5P (atmosphere), and Sentinel-6 (altimetry) collections with temporal, spatial, and attribute filters
- **Geographic Search** — Find satellite products covering any location on Earth using bounding box coordinates or WKT polygon geometries
- **Orbit-Based Queries** — Retrieve data from specific satellite orbits for interferometry, change detection, and repeat-pass analysis
- **Product Inspection** — Access complete metadata, quicklook previews, and internal file structure for any product
- **Download Orchestration** — Generate authenticated download URLs with time-limited Bearer tokens for direct product retrieval
- **Data Volume Assessment** — Count products matching your criteria before executing full searches

### How it works

1. Subscribe to this server
2. Register at [dataspace.copernicus.eu](https://dataspace.copernicus.eu/) and create an OAuth2 client
3. Enter your credentials as `client_id:client_secret` in the field below
4. Start querying terabytes of satellite data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Remote Sensing Analysts** — discover and access satellite imagery for land use mapping, urban planning, and environmental monitoring
- **Climate Researchers** — query long-term data archives for climate change analysis and carbon monitoring
- **Agriculture Professionals** — find cloud-free imagery for precision farming, crop monitoring, and yield estimation
- **Emergency Response Teams** — rapidly locate recent satellite acquisitions for disaster assessment and situational awareness


## Available Tools
- **check_copernicus_status**: Returns the connection status. Use this to verify your client_id:client_secret credentials are working correctly.

Verify Copernicus Data Space API connectivity and authentication
- **count_products**: Useful for understanding data volume before executing a full search, or for monitoring data availability trends.

Count total products available for a collection and date range
- **get_collection**: Use collection names like "SENTINEL-2", "SENTINEL-1", or "SENTINEL-3".

Get details about a specific Copernicus collection
- **get_product_download_url**: Returns the direct download URL along with a Bearer token valid for approximately one hour. Use this to download raw satellite data products (typically in SAFE format for Sentinel data).

Generate an authenticated download URL for a product
- **get_product**: Returns name, sensing time, footprint geometry, file size, checksum, and all associated attributes. Use this after searching to inspect a specific product before downloading.

Get detailed metadata for a specific satellite product by UUID
- **get_quicklook**: Useful for understanding the product structure and accessing thumbnail previews without downloading the full product.

Get quicklook preview and file nodes for a product
- **list_attributes**: This helps you understand what filtering parameters are available (e.g., cloud cover percentage, orbit direction, processing level) for refining product searches.

List available metadata attributes for a collection
- **list_collections**: Includes Sentinel-1 (radar), Sentinel-2 (optical), Sentinel-3 (ocean/land), Sentinel-5P (atmosphere), Sentinel-6 (altimetry), and complementary missions like Landsat. Each entry includes temporal coverage and description.

List all available Copernicus satellite data collections
- **list_latest_products**: Useful for monitoring new data availability or checking processing pipeline status.

List the most recently published satellite products
- **list_product_nodes**: Returns the hierarchy of files including measurement data, metadata XML, quicklook images, and auxiliary data. Essential for understanding product structure before selective download.

List all files contained within a satellite product
- **search_by_bbox**: Combines spatial filtering with collection and temporal constraints. Ideal for region-specific analysis workflows.

Search satellite products within a geographic bounding box
- **search_by_name**: Useful for finding specific orbits, tiles (e.g., "T33UUP" for Sentinel-2 tile), or granule identifiers. Returns product metadata ordered by sensing date.

Search satellite products by name pattern
- **search_by_orbit_number**: Especially useful for Sentinel-1 (SAR) and Sentinel-2 (optical) repeat-pass analysis, interferometry, and change detection workflows where you need data from the exact same orbit geometry.

Search satellite products by orbit number
- **search_products**: Specify a collection name (e.g., "SENTINEL-2", "SENTINEL-1"), a date range in YYYY-MM-DD format, and optionally an area of interest as a WKT polygon. Returns product metadata including name, footprint, size, and publication date. Maximum 20 results by default.

Search Sentinel satellite products by collection, date range, and area


## Installation & Usage

To install and use the **Copernicus Data Space** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copernicus-data-space](https://vinkius.com/mcp/copernicus-data-space)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
