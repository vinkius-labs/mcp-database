# Maxar (Satellite Imagery) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maxar-satellite-imagery)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access high-resolution satellite imagery and geospatial data from Maxar — search discovery catalogs, order data products, and retrieve streaming endpoints.

## Description
Connect to **Maxar**, the world leader in high-resolution satellite imagery, and integrate earth intelligence directly into your AI workflows. This server allows you to query the Maxar Discovery Service, manage orders, and access OGC-compliant streaming services.

### What you can do

- **Imagery Discovery** — Search for available satellite imagery using spatial bounding boxes, temporal filters, and specific satellite collections (like WorldView-3).
- **Product Ordering** — Request delivery of specific imagery products (visual, multispectral, or panchromatic) directly to your cloud storage.
- **ARD Metadata** — Retrieve detailed metadata for Analysis Ready Data (ARD) tiles to streamline your geospatial analysis.
- **Streaming Access** — Get base URLs for OGC-compliant streaming services (WMS, WMTS) to visualize imagery in GIS applications or custom dashboards.

### How it works

1. Subscribe to this server
2. Enter your Maxar Client ID and Client Secret
3. Start querying the planet from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Geospatial Analysts** — Quickly find and inspect imagery for specific regions without leaving your analysis environment.
- **Data Scientists** — Automate the discovery and ordering of training data for machine learning models.
- **GIS Developers** — Retrieve streaming endpoints and tile metadata to power custom mapping applications.


## Available Tools
- **create_order**: Order specific data products
- **get_mws_endpoints**: Get Maxar Web Services (MWS) endpoints
- **list_order_pipelines**: List available ordering pipelines
- **search_discovery**: Search for available satellite imagery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maxar (Satellite Imagery)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for available satellite imagery in the bbox [-122.5, 37.7, -122.3, 37.8] from the last 6 months."

**🤖 AI Agent:**
> I've searched the Maxar Discovery Service. I found several high-quality images from the WV03_VNIR collection. The most recent one was captured on 2024-05-15 with 0% cloud cover. Would you like the full metadata for this item?

---

**👤 You:**
> "Get the streaming endpoints for Maxar Web Services."

**🤖 AI Agent:**
> I have retrieved the OGC endpoints for you. You can use the following base URLs for streaming: WMS: `https://securewatch.maxar.com/mapservice/wms...` and WMTS: `https://securewatch.maxar.com/mapservice/wmts...`. You will need to append your credentials to these URLs for use in GIS tools.

---

**👤 You:**
> "Retrieve metadata for the ARD tile with ID '1234567890'."

**🤖 AI Agent:**
> Fetching ARD tile metadata... Tile '1234567890' is part of the 'Bay Area' dataset, processed on 2024-01-10. It includes 8-band multispectral data and has been orthorectified to UTM Zone 10N.


## ❓ FAQ

**Q: How do I search for satellite imagery in a specific geographic area?**
You can use the `search_discovery` tool by providing a bounding box (bbox) array with [min_lon, min_lat, max_lon, max_lat] coordinates and an optional datetime interval.

**Q: Can I get streaming links for use in GIS software like QGIS or ArcGIS?**
Yes! Use the `get_mws_endpoints` tool to retrieve the base URLs for OGC-compliant WMS and WMTS services provided by Maxar Web Services.

**Q: What information is required to order a specific image?**
To use the `create_order` tool, you need the unique `item_id` of the image, the desired `product_type` (e.g., visual), and a `delivery_config` JSON specifying the destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maxar-satellite-imagery](https://vinkius.com/mcp/maxar-satellite-imagery)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maxar (Satellite Imagery)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `maxar-satellite-imagery` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maxar (Satellite Imagery)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maxar-satellite-imagery": {
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
