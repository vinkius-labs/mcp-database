# ArcGIS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcgis-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access GIS services via ArcGIS — geocode addresses, search places, get routes, check elevation and discover basemap styles from any AI agent.

## Description
Connect to **ArcGIS** location services through any AI agent and explore geographic data through natural conversation.

### What you can do

- **Geocoding** — Convert street addresses and place names to coordinates (lat/lon) with high accuracy
- **Reverse Geocoding** — Convert GPS coordinates to human-readable addresses
- **Place Search** — Find nearby points of interest (restaurants, hotels, gas stations, hospitals) by category
- **Routing** — Calculate driving directions between locations with distance and travel time
- **Elevation** — Get elevation data for any location on Earth
- **Basemap Styles** — Discover available map styles for visualization projects

### How it works

1. Subscribe to this server
2. Enter your ArcGIS API Key
3. Start exploring geographic data from Claude, Cursor, or any MCP-compatible client

No more navigating complex GIS software to find coordinates or calculate routes. Your AI acts as a dedicated geospatial analyst.

### Who is this for?

- **Developers** — quickly geocode addresses, calculate routes and find places without writing complex GIS code
- **Analysts** — explore elevation data, reverse geocode coordinates and discover nearby points of interest
- **Travel Planners** — get driving directions, estimate travel times and find places along the route
- **Researchers** — access geographic data for academic work, urban planning and geographic studies


## Available Tools
- **geocode_address**: Accepts free-form address text like "1600 Pennsylvania Ave, Washington DC" or "Eiffel Tower, Paris". Returns candidate matches with coordinates, address components and confidence scores. Useful for mapping and location-based queries.

Geocode an address to coordinates
- **get_basemap_styles**: Each style includes its name, description, thumbnail URL and style ID. Useful for discovering map styles for visualization projects.

List available basemap styles
- **get_elevation**: Accepts locations as semicolon-separated "longitude,latitude" pairs. Returns elevation in meters for each location. Useful for terrain analysis, hiking planning and geographic research.

Get elevation data for locations
- **get_route**: Stops are specified as semicolon-separated "longitude,latitude" pairs (e.g. "-77.0365,38.8977;-74.0060,40.7128" for Washington DC to NYC). Optionally set travel mode (driving, trucking, walking). Returns route geometry, total distance, total travel time and turn-by-turn directions.

Get driving directions between stops
- **reverse_geocode**: Accepts location as "longitude,latitude" (e.g. "-77.0365,38.8977" for Washington DC). Returns the nearest address, place name and location details. Useful for identifying locations from GPS coordinates.

Reverse geocode coordinates to address
- **search_places**: Accepts a location ("longitude,latitude") and optional category (e.g. "Coffee Shop", "Restaurant", "Gas Station", "Hotel", "Hospital") and search radius in meters. Returns nearby places with names, addresses, categories and distances.

Search for places near a location


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ArcGIS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geocode the address '1600 Pennsylvania Ave, Washington DC'."

**🤖 AI Agent:**
> Found: 1600 Pennsylvania Ave NW, Washington, DC 20500 at coordinates -77.0365, 38.8977. Confidence: 100%. This is the White House.

---

**👤 You:**
> "Find coffee shops near San Francisco coordinates -122.4194,37.7749."

**🤖 AI Agent:**
> Found 8 coffee shops within 1km: Blue Bottle Coffee (0.2km), Sightglass Coffee (0.3km), Ritual Coffee Roasters (0.4km), Four Barrel Coffee (0.5km), and 4 more. Each with address and distance info.

---

**👤 You:**
> "Get driving directions from Washington DC to New York City."

**🤖 AI Agent:**
> Route from DC to NYC: 225 miles, estimated 3 hours 45 minutes driving time. Route goes through Baltimore, Philadelphia and into Manhattan. Total tolls approximately $45.


## ❓ FAQ

**Q: How do I get an ArcGIS API key?**
Log in to the [**ArcGIS Developer Dashboard**](https://developers.arcgis.com/dashboard/), create or select an application, and generate an API key. Configure the scopes you need (geocoding, routing, places, elevation). Free tier includes generous usage limits.

**Q: Can I calculate driving directions?**
Yes! Use `get_route` with stops specified as semicolon-separated longitude,latitude pairs. For example, '-77.0365,38.8977;-74.0060,40.7128' for Washington DC to NYC. Optionally set travel mode to Driving, Trucking or Walking.

**Q: Can I find nearby places?**
Yes! Use `search_places` with a location (longitude,latitude) and optionally a category like 'Coffee Shop', 'Restaurant', 'Gas Station' or 'Hotel'. Set the radius in meters to control the search area. Returns places with names, addresses, categories and distances.

**Q: Can I get elevation data?**
Yes! Use `get_elevation` with locations specified as semicolon-separated longitude,latitude pairs. Returns elevation in meters for each location. You can query multiple locations in a single request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcgis-alternative](https://vinkius.com/mcp/arcgis-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ArcGIS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `arcgis-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ArcGIS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arcgis-alternative": {
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
