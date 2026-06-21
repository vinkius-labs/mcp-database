# Mapbox MCP Server

Geocode addresses, get directions, calculate distances and generate maps with Mapbox's location platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mapbox)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 8

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


## Installation & Usage

To install and use the **Mapbox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapbox](https://vinkius.com/mcp/mapbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
