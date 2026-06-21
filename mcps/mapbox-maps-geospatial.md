# Mapbox (Maps & Geospatial) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapbox-maps-geospatial)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build with location data via Mapbox — geocode addresses, calculate routes, and solve trip optimization.

## Description
Connect your **Mapbox** account to any AI agent and take full control of world-class geocoding, navigation, and geospatial intelligence through natural conversation.

### What you can do

- **Geocoding & Search** — Convert text addresses into precise geographic coordinates (GeoJSON) or perform reverse lookups to identify locations from GPS points directly
- **Advanced Routing** — Calculate driving, walking, or cycling directions between up to 25 points, including real-time traffic-aware ETA and turn-by-turn navigation data
- **Trip Optimization** — Solve the Traveling Salesperson Problem (TSP) by determining the most efficient order to visit multiple coordinates to minimize travel time
- **Isochrone Analysis** — Compute reachable area polygons within specific travel times (e.g., 'What areas are within a 15-minute walk?') for urban planning and delivery logic
- **Road Snapping** — Align noisy or distorted GPS traces perfectly onto the road network using native map matching configurations for accurate tracking
- **Geospatial Intelligence** — Query high-resolution elevation data for any coordinate or generate static map image URLs for rapid visual verification
- **Logistics Matrices** — Compute all-to-all travel times and distances between multiple origins and destinations to optimize fleet management workflows

### How it works

1. Subscribe to this server
2. Enter your Mapbox Access Token
3. Start building location-aware applications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — integrate mapping and navigation services into AI agents and validate geocoding results through natural conversation
- **Logistics Managers** — optimize delivery routes and calculate distance matrices for fleets without manual GIS software
- **Data Analysts** — clean GPS datasets using road snapping and enrich location data with precise elevation and coordinate metadata


## Available Tools
- **get_directions**: Calculate driving, walking, or cycling directions between points
- **get_elevation**: Query elevation data for a specific coordinate point
- **search_places**: Search for places, addresses, or POIs using Mapbox Geocoding
- **get_isochrones**: Calculate reachable areas within a specific travel time
- **snap_to_road**: Snap noisy GPS traces sequentially to a road network
- **get_distance_matrix**: Calculate a distance and travel time matrix between many points
- **solve_optimization**: Solve trip optimization (Traveling Salesperson Problem)
- **reverse_geocode**: Perform reverse geocoding to find places or addresses at a specific coordinate
- **geocoding_session**: Perform autocomplete geocoding operations attached to a session
- **generate_static_map**: Generate a static map image URL centered on coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mapbox (Maps & Geospatial)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the coordinates for 'Golden Gate Bridge' in San Francisco"

**🤖 AI Agent:**
> Resolving place… I've found the Golden Gate Bridge at latitude 37.8199 and longitude -122.4783. It is classified as a POI (Point of Interest). Would you like me to find driving directions to this location?

---

**👤 You:**
> "Get driving directions from New York to Philadelphia with traffic-aware ETA"

**🤖 AI Agent:**
> Calculating route… The optimal path via I-95 S is approximately 152 km. With current traffic conditions, the estimated travel time is 1 hour and 45 minutes. I can provide the detailed turn-by-turn navigation data if you'd like.

---

**👤 You:**
> "What areas are within a 5-minute walk from '-73.9857,40.7484'?"

**🤖 AI Agent:**
> Computing isochrone… I've generated a 5-minute walking polygon centered near the Empire State Building. This area covers approximately 0.8 square kilometers. Would you like me to provide the GeoJSON coordinates for this reachable zone?


## ❓ FAQ

**Q: Can I calculate which areas are reachable within a 10-minute drive through my agent?**
Yes. Use the `get_isochrones` tool by providing the center coordinates and '10' as the minutes parameter. Your agent will return GeoJSON polygons representing the reachable areas for the specified profile (driving, walking, or cycling).

**Q: How do I optimize a delivery route with multiple stops through a conversation?**
The `solve_optimization` tool determines the most efficient order to visit a list of coordinates. Your agent will process the request and return the optimized sequence, minimizing either travel time or distance for your logistics workflow.

**Q: Can my agent generate a map image for a specific location?**
Absolutely. Use the `generate_static_map` tool by specifying the center, zoom, and resolution. Your agent will provide a usable Mapbox static image URL, perfect for visual verification without needing a mapping library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapbox-maps-geospatial](https://vinkius.com/mcp/mapbox-maps-geospatial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mapbox (Maps & Geospatial)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mapbox-maps-geospatial` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mapbox (Maps & Geospatial)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapbox-maps-geospatial": {
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
