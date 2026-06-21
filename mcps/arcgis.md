# ArcGIS MCP Server

Automate mapping and spatial analysis via ArcGIS — perform geocoding, route solving, vehicle routing, and calculate origin-destination matrices from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arcgis)

## Overview
**Category:** superpower
**Tools Count:** 10

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


## Installation & Usage

To install and use the **ArcGIS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcgis](https://vinkius.com/mcp/arcgis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
