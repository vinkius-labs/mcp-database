# Mapbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapbox-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Integrate Mapbox mapping and location services into your AI agent—access vector/raster tiles, static images, directions, and manage datasets.

## Description
Connect your **Mapbox** account to any AI agent to leverage powerful geospatial capabilities through natural language.

### What you can do

- **Maps & Tiles** — Retrieve vector and raster tiles or generate standalone static map images for specific coordinates and styles.
- **Navigation & Routing** — Calculate optimal routes with turn-by-turn instructions and travel time matrices between multiple locations.
- **Dataset Management** — List, retrieve, and update features within your Mapbox datasets directly from the conversation.
- **Tileset Publishing** — Create and publish tileset sources using the Mapbox Tiling Service (MTS) for custom map layers.
- **Spatial Queries** — Use Tilequery to retrieve detailed data about specific features at any given longitude and latitude.

### How it works

1. Subscribe to this server
2. Enter your Mapbox Access Token (Public or Secret)
3. Start querying maps, directions, and geospatial data from Claude, Cursor, or any MCP client

### Who is this for?

- **GIS Specialists & Developers** — quickly inspect dataset features and tileset statuses without leaving the terminal or editor.
- **Logistics Managers** — calculate routes and travel matrices to optimize fleet movements via simple AI prompts.
- **Data Analysts** — perform spatial queries and retrieve feature metadata for geographic research and reporting.


## Available Tools
- **geocode_reverse**: Reverse geocoding (v6)
- **get_dataset_feature**: Retrieve a specific feature from a dataset
- **get_directions**: Calculate optimal routes and turn-by-turn instructions
- **get_feedback**: Get user feedback
- **get_isochrone**: Computes reachable areas within a specified time or distance
- **get_map_matching**: Snaps fuzzy GPS traces to the road network
- **get_matrix**: Returns travel times or distances between many points
- **get_optimization**: Retrieve a previously submitted optimization solution
- **get_raster_tile**: png, .jpg, .webp, .grid.json) from a Mapbox-hosted tileset.

Get a raster tile from Mapbox
- **create_tileset_source**: Create a Mapbox Tiling Service (MTS) source
- **create_token**: Create a new access token
- **delete_token**: Delete an access token
- **geocode_batch**: Batch geocoding (v6)
- **geocode_forward**: Forward geocoding (v6)
- **get_static_image**: Get a static map image
- **get_tilequery**: Retrieve data about specific features from tilesets at a point
- **get_vector_tile**: mvt or .vector.pbf) from a Mapbox-hosted tileset.

Get a vector tile from Mapbox
- **list_datasets**: List Mapbox datasets for a user
- **list_tokens**: List access tokens for a user
- **publish_tileset**: Publish a Mapbox Tiling Service (MTS) tileset
- **searchbox_forward**: Forward search using the Search Box API
- **searchbox_retrieve**: Retrieve full details for a searchbox suggestion
- **searchbox_reverse**: Reverse search using the Search Box API
- **searchbox_suggest**: Interactive location search with autocomplete
- **submit_feedback**: Submit user feedback
- **submit_optimization**: Solves the Traveling Salesperson Problem for fleet routing
- **update_dataset_feature**: Update a specific feature in a dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mapbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a driving route between -74.006,40.7128 and -71.0589,42.3601."

**🤖 AI Agent:**
> I've calculated the route from New York to Boston. The optimal path covers approximately 215 miles with an estimated travel time of 3 hours and 45 minutes via I-95 N.

---

**👤 You:**
> "Generate a static map image for San Francisco at zoom level 12."

**🤖 AI Agent:**
> I've generated the static map for San Francisco (Lon: -122.4194, Lat: 37.7749) at zoom 12. You can view the image here: [Map Image URL].

---

**👤 You:**
> "List all my Mapbox datasets for username 'dev_user'."

**🤖 AI Agent:**
> I found 3 datasets for 'dev_user': 'city-parks-v1' (ID: cl123...), 'office-locations' (ID: cl456...), and 'transit-routes' (ID: cl789...). Which one would you like to inspect?


## ❓ FAQ

**Q: Can I calculate driving directions between two points using this server?**
Yes! Use the `get_directions` tool. You need to provide a routing profile (like `mapbox/driving`) and the coordinates as a semicolon-separated string of longitude and latitude.

**Q: How do I find information about map features at a specific coordinate?**
You can use the `get_tilequery` tool. By providing a tileset ID and the longitude/latitude, the agent will retrieve data about the specific features located at that point.

**Q: Is it possible to update my Mapbox datasets through the AI?**
Yes, the `update_dataset_feature` tool allows you to modify a specific feature within a dataset by providing the dataset ID, feature ID, and the new GeoJSON data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapbox-alternative](https://vinkius.com/mcp/mapbox-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mapbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mapbox-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mapbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapbox-alternative": {
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
