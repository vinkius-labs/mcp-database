# Mapbox (Maps & Geospatial) MCP Server

Build with location data via Mapbox — geocode addresses, calculate routes, and solve trip optimization.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mapbox-maps-geospatial)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Mapbox (Maps & Geospatial)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapbox-maps-geospatial](https://vinkius.com/mcp/mapbox-maps-geospatial)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
