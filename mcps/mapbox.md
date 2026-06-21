# Mapbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mapbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Geocode addresses, get directions, calculate distances and generate maps with Mapbox's location platform.

## Description
Connect to **Mapbox** and access world-class location services through natural conversation.

### What you can do

- **Geocoding** — Convert addresses, place names and POIs to coordinates and structured addresses
- **Reverse Geocoding** — Convert GPS coordinates to human-readable addresses
- **Directions** — Get driving, walking and cycling routes with step-by-step instructions
- **Distance Matrix** — Calculate travel times and distances between multiple locations
- **Isochrones** — Show areas reachable within a specific time or distance
- **Elevation** — Get elevation data for any coordinates
- **Static Maps** — Generate map image URLs for any location
- **Nearby Search** — Find points of interest near coordinates

### How it works

1. Subscribe to this server
2. Enter your Mapbox Access Token
3. Start using location services from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — geocode addresses, calculate routes and generate map images via API
- **Logistics** — optimize delivery routes with distance matrices and isochrones
- **Travelers** — get directions, find nearby places and check elevation data


## Available Tools
- **geocode**: Returns the place name, coordinates, address components (street, city, state, postal code, country), place type and bounding box. Use this to find coordinates for use with directions, distance matrix and other tools.

Convert a place name to coordinates
- **get_directions**: Returns route distance, duration, geometry, step-by-step instructions and maneuver data. Supports driving (mapbox/driving), walking (mapbox/walking) and cycling (mapbox/cycling) profiles. Coordinates are semicolon-separated "longitude,latitude" pairs (e.g. "-77.0365,38.8977;-74.006,40.7128" for DC to NYC).

Get driving, walking or cycling directions
- **get_distance_matrix**: Useful for logistics, delivery routing and travel planning. Returns a matrix of durations (seconds) and distances (meters) between all source-destination pairs. Coordinates are semicolon-separated "lon,lat" pairs. Supports driving, walking and cycling profiles.

Get travel times between multiple origins and destinations
- **get_elevation**: Useful for hiking, aviation and geographic research. Coordinates are comma-separated "lon,lat" pairs.

Get elevation for coordinates
- **get_isochrone**: Returns polygon contours showing the reachable area. Useful for determining service areas, commute ranges and accessibility. Coordinates are "lon,lat".

Get reachable area within a time or distance
- **get_static_map**: Returns a direct image URL that can be used in markdown, HTML or downloaded. Supports customizable zoom level and image dimensions.

Generate a static map image for a location
- **reverse_geocode**: Returns the nearest address, city, state, country and other location details.

Convert coordinates to an address
- **search_nearby**: Returns nearby places with names, addresses, categories, distances and coordinates. Use query to search for specific types of places (e.g. "restaurant", "gas station", "hotel").

Search for places near coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mapbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geocode '1600 Pennsylvania Ave, Washington DC'."

**🤖 AI Agent:**
> Found: The White House at 38.8977°N, 77.0365°W. Full address: 1600 Pennsylvania Avenue NW, Washington, DC 20500, United States. Place type: address. Bounding box provided.

---

**👤 You:**
> "Get driving directions from San Francisco to Los Angeles."

**🤖 AI Agent:**
> Route from San Francisco to Los Angeles: 616 km (383 miles), estimated 5 hours 50 minutes via I-5 S. Step-by-step instructions include: Head south on Market St, merge onto US-101 S, continue on I-5 S to Los Angeles.

---

**👤 You:**
> "Show me the area reachable within 15 minutes driving from Times Square, NYC."

**🤖 AI Agent:**
> Within 15 minutes driving from Times Square you can reach: most of Manhattan below 96th St, parts of Brooklyn (Williamsburg, DUMBO), Long Island City in Queens, and parts of the Bronx via the bridges. The isochrone polygon covers approximately 85 square km.


## ❓ FAQ

**Q: How do I get a Mapbox Access Token?**
Sign up for a free account at [**account.mapbox.com**](https://account.mapbox.com/access-tokens/), go to **Access Tokens** and create a new token. Copy the token — it starts with `pk.`.

**Q: Can I get driving directions?**
Yes! Use get_directions with coordinates and the 'driving' profile. Returns route distance, duration, step-by-step instructions and geometry. Also supports 'walking' and 'cycling' profiles.

**Q: What are isochrones used for?**
Isochrones show the area reachable within a specific time or distance from a location. Useful for delivery zones, commute analysis, real estate proximity and accessibility planning.

**Q: Can I calculate distances between multiple locations?**
Yes! Use get_distance_matrix with multiple coordinate pairs. Returns a matrix of durations (seconds) and distances (meters) between all source-destination pairs. Supports driving, walking and cycling profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapbox](https://vinkius.com/mcp/mapbox)
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
3. Set Type to "SSE", enter `mapbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mapbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mapbox": {
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
