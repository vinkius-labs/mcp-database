# Copernicus Data Space MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/copernicus-data-space)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access satellite imagery and Earth observation datasets from the EU Copernicus program for environmental and geospatial analysis.

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


## Available Tools (14)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copernicus Data Space** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find Sentinel-2 satellite images over Lisbon from the last week."

**🤖 AI Agent:**
> Searching the Copernicus catalogue for SENTINEL-2 products over Lisbon... I found 8 products in the last 7 days. The most recent is S2B_MSIL2A acquired yesterday with 12% cloud cover. The cleanest scene has only 3% cloud cover from 3 days ago. Would you like me to get the download URL for the cloud-free scene?

---

**👤 You:**
> "How many Sentinel-1 radar products are available for January 2026?"

**🤖 AI Agent:**
> Counting SENTINEL-1 products for January 2026... The catalogue contains 42,738 products for that period. Sentinel-1 acquires radar imagery regardless of cloud cover or daylight, so coverage is continuous. Would you like me to search for products in a specific region?

---

**👤 You:**
> "What data collections are available in the Copernicus Data Space?"

**🤖 AI Agent:**
> Fetching available collections... The Copernicus Data Space currently hosts 15 data collections including SENTINEL-1 (C-band SAR radar), SENTINEL-2 (multispectral optical at 10-60m), SENTINEL-3 (ocean color and land surface), SENTINEL-5P (tropospheric monitoring), SENTINEL-6 (precise ocean altimetry), plus Landsat-5/7/8/9, SMOS, MERIS, and DEM datasets. Would you like details about a specific collection?


## ❓ FAQ

**Q: How do I get Copernicus OAuth2 credentials?**
Register for free at dataspace.copernicus.eu, navigate to your User Settings dashboard, and create a new OAuth client. You'll receive a Client ID and Client Secret — enter them in the format client_id:client_secret. The entire process takes under 2 minutes.

**Q: What satellite data is available through this server?**
You can access data from all Copernicus Sentinel missions: Sentinel-1 (SAR radar imagery), Sentinel-2 (high-resolution optical imagery at 10m), Sentinel-3 (ocean and land monitoring), Sentinel-5P (atmospheric composition), Sentinel-6 (sea level altimetry), plus complementary data from Landsat, SMOS, and MERIS missions.

**Q: Can I download satellite products through this server?**
Yes. Use the get_product_download_url tool with a product UUID to generate a time-limited authenticated download URL. The URL and Bearer token are valid for approximately one hour. Products are typically in ESA SAFE format and can range from hundreds of megabytes to several gigabytes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/copernicus-data-space](https://vinkius.com/mcp/copernicus-data-space)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copernicus Data Space** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `copernicus-data-space` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copernicus Data Space** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copernicus-data-space": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
