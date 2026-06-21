# ArcGIS MCP Server

Access GIS services via ArcGIS — geocode addresses, search places, get routes, check elevation and discover basemap styles from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/arcgis-alternative)

## Overview
**Category:** industry-titans
**Tools Count:** 6

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


## Installation & Usage

To install and use the **ArcGIS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcgis-alternative](https://vinkius.com/mcp/arcgis-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
