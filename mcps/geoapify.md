# Geoapify MCP Server

Access powerful location intelligence — geocoding, routing, place search, and IP tracking directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/geoapify)

## Overview
**Category:** data-analytics
**Tools Count:** 17

## Description
Integrate **Geoapify** into your AI workflows to provide your agent with advanced geospatial capabilities. From simple address lookups to complex route matrix calculations, this server enables precise location-based decision making.

### What you can do

- **Geocoding & Search** — Convert addresses to coordinates with `geocode_search` or get real-time suggestions using `geocode_autocomplete`.
- **Reverse Geocoding** — Identify human-readable addresses from GPS coordinates using `geocode_reverse`.
- **Routing & Logistics** — Calculate optimal paths with `calculate_route` or generate distance matrices for multiple origins and destinations via `calculate_route_matrix`.
- **Location Intelligence** — Detect user regions via `get_ip_info` or find specific points of interest with `search_places`.
- **Map Matching** — Snap messy GPS tracks to the actual road network using `map_matching` for precise fleet tracking.

### How it works

1. Subscribe to this server
2. Enter your Geoapify API Key
3. Start querying location data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — automate route planning and distance calculations for delivery fleets.
- **Developers** — implement address validation and autocomplete features without leaving the IDE.
- **Data Analysts** — enrich datasets with precise coordinates, elevation data, and administrative boundaries.


## Available Tools
- **calculate_isoline**: Calculate areas reachable within a certain time (isochrones) or distance (isodistances)
- **calculate_route_matrix**: Calculate travel times and distances between multiple sources and targets
- **calculate_route**: Calculate routes for various modes (drive, truck, bicycle, walk, transit)
- **create_batch_job**: Process up to 1000 requests in a single asynchronous job
- **geocode_autocomplete**: Get real-time suggestions for address input fields
- **geocode_reverse**: Find the address for a specific GPS coordinate
- **geocode_search**: Convert free-form or structured addresses into coordinates
- **geometry_operation**: Perform spatial operations on GeoJSON data (union, intersection, buffer, etc.)
- **get_batch_job**: Get results for an asynchronous batch job
- **get_boundaries_consists_of**: Retrieve sub-boundaries within an area
- **get_boundaries_part_of**: Retrieve administrative, postal, or political boundaries containing a point
- **get_elevation**: Get elevation data for specific coordinates
- **get_place_details**: Get detailed info (contact, opening hours, building geometry) for a place
- **get_ip_info**: Detect user location based on IP address
- **map_matching**: Snap GPS tracks to the road network
- **route_planner**: Solve Vehicle Routing Problems (VRP), including TSP and delivery optimization
- **search_places**: Find points of interest (POIs) by category


## Installation & Usage

To install and use the **Geoapify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geoapify](https://vinkius.com/mcp/geoapify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
