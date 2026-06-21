# ArcGIS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcgis)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arcgis-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arcgis-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Automate mapping and spatial analysis via ArcGIS — perform geocoding, route solving, vehicle routing, and calculate origin-destination matrices from any AI agent.

## Description
Connect your **ArcGIS** account to any AI agent and take full control of your location and spatial intelligence through natural conversation.

### What you can do

- **Geocoding & Reverse Geocoding** — Convert street addresses to coordinates instantly or discover the closest address to a specific longitude/latitude pair
- **Batch Geocoding** — Process bulk batches of up to 1000 geographical addresses in a single AI operation
- **Route Solving** — Calculate the optimal route between multiple stops, complete with turn-by-turn directions, travel time, and precise distances
- **Vehicle Routing** — Solve complex Vehicle Routing Problems (VRP) to optimize fleets and logistics deliveries
- **Service Area Analysis** — Calculate drive-time, walk-time, or travel-distance polygons reachable from a specific facility
- **Origin-Destination Matrices** — Compute travel constraints and cost matrices between multiple origins and tracking destinations

### How it works

1. Subscribe to this server
2. Enter your ArcGIS Developer API Key
3. Start exploring and calculating spatial data from Claude, Cursor, or any MCP-compatible client

No more switching tabs to specialized GIS dashboards. Your AI agent acts as a fully integrated geoprocessing command center.

### Who is this for?

- **Logistics teams** — optimize fleet routes, trace deliveries, and calculate exact driving times without leaving your operations workflow
- **Retail businesses** — map out service areas and understand the geographic reach of your new store locations
- **Real estate agents** — automate batch address queries and enrich property listings with hyper-local context
- **Data scientists** — clean and resolve coordinate anomalies using the powerful ArcGIS suggestion engine


## Available Tools
- **calculate_service_area**: Facilities specified as lon,lat.

Calculate drive-time, walk-time, or travel-distance service areas
- **find_address_country**: g., USA, BRA, FRA). Ensures results are geographically bounded.

Find an address filtered by a specific country
- **find_address_candidates**: Use this to turn text addresses into latitude and longitude.

Find an address or place using ArcGIS Geocoding
- **batch_geocode_addresses**: Addresses must be provided as an ArcGIS-compatible JSON array string.

Geocode a bulk batch of up to 1000 addresses
- **calculate_od_matrix**: Calculate travel time and distances between multiple origins and destinations
- **reverse_geocode**: Coordinate format must be lon,lat (e.g. -117.19,34.05).

Discover the closest address to a specific location (lon,lat)
- **solve_nav_route**: Point sequence must be provided as lon,lat;lon,lat. Returns detailed turn-by-turn directions, travel time, and distance.

Find the best route between two or more locations
- **solve_vehicle_routing**: Takes an ArcGIS Orders JSON mapping string detailing the stops.

Solve a Vehicle Routing Problem (VRP) for a fleet
- **suggest_location_bias**: Get autocomplete suggestions biased towards a specific location
- **suggest_geocoding**: Use this to help users select valid addresses before performing a full geocode request.

Get autocomplete suggestions for partial addresses or place names


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ArcGIS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the closest address to coordinates -117.19, 34.05?"

**🤖 AI Agent:**
> Running a reverse geocode... The closest address to (-117.19, 34.05) is 380 New York St, Redlands, California, 92373. Would you like me to calculate a service area originating from this point?

---

**👤 You:**
> "Find the optimal driving route visiting stops -122.4,37.7 and -122.5,37.8."

**🤖 AI Agent:**
> I've solved the route using the ArcGIS engine. The optimal path takes approximately 28 minutes covering 14.5 miles. The first turn is head north on 4th St toward Mission St. I can provide the full turn-by-turn breakdown if needed.

---

**👤 You:**
> "Resolve the coordinate location for 'Central Park' but restrict the search strictly to the USA."

**🤖 AI Agent:**
> Using the country-filtered search, 'Central Park' resolves to -73.96, 40.78 (New York City, New York, USA). Bounding the search to the USA avoided matching international places with similar names.


## Installation & Usage

To install and use the **ArcGIS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcgis](https://vinkius.com/mcp/arcgis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
