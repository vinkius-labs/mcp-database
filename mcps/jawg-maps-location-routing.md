# Jawg Maps (Location & Routing) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jawg-maps-location-routing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jawg-maps-location-routing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jawg-maps-location-routing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Build with location data via Jawg Maps — search places, calculate routes, compute distance matrices, and get elevation data.

## Description
Connect your **Jawg Maps** account to any AI agent and take full control of professional map services and geospatial analytics through natural conversation.

### What you can do

- **Place Search & Geocoding** — Find addresses and points of interest (POI) by text or resolve GPS coordinates to physical locations directly from your agent
- **Advanced Routing** — Calculate optimal paths for driving, biking, or walking with support for multiple waypoints and transportation profiles
- **Distance Matrices** — Compute massive travel time and distance tables between multiple origins and destinations for logistics optimization
- **Reachability Isochrones** — Visualize reachable areas from a center point based on precise travel time or distance limits (drive-time polygons)
- **Elevation Profiles** — Retrieve the altitude and elevation above sea level for specific coordinates or along a calculated route path
- **Geo-Filtering** — Perform restricted searches within specific ISO country borders to ensure data accuracy and regional compliance

### How it works

1. Subscribe to this server
2. Enter your Jawg Access Token
3. Start building location-aware applications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **GIS Developers** — integrate geocoding and routing services into AI agents and test API results through natural conversation
- **Logistics Planners** — calculate optimal routes and distance matrices for delivery fleets and supply chain management
- **Urban Researchers** — analyze city accessibility and elevation data across different geographic regions efficiently


## Available Tools
- **search_autocomplete**: You can optionally bias results towards a specific GPS location.

Autocomplete a place or address search query
- **calculate_elevation_routing**: Calculate a route that includes elevation profiles
- **get_path_elevation**: Get elevation data for specific coordinates
- **calculate_distance_isochrone**: Calculate the area reachable within a given distance limit
- **calculate_reachability_isochrone**: Calculate the area reachable within a given time limit
- **calculate_distance_matrix**: Compute travel times and distances between multiple origins and destinations
- **reverse_geocode**: Get address information from GPS coordinates
- **calculate_routing_line**: ) passing through the provided waypoints.

Calculate a route between multiple coordinates
- **search_country_filter**: Search for places with a strict country filter
- **search_map_places**: Returns matching locations with their coordinates.

Search for places and addresses by text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jawg Maps (Location & Routing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the physical address for coordinates 48.8566, 2.3522"

**🤖 AI Agent:**
> Resolving coordinates… That location corresponds to '2 Place de l'Hôtel de Ville, 75004 Paris, France'. It's categorized as a City Hall. Would you like to see nearby points of interest?

---

**👤 You:**
> "Calculate a driving route from Paris to Lyon via Dijon"

**🤖 AI Agent:**
> Calculating route… The optimal path via A6 is approximately 465 km and will take about 4 hours and 20 minutes with standard traffic. I've included the waypoints for Dijon in the calculation. Would you like the turn-by-turn summary?

---

**👤 You:**
> "Show me the elevation for these coordinates: 45.8326, 6.8651"

**🤖 AI Agent:**
> Retrieving elevation data… Those coordinates (near Mont Blanc) have an altitude of approximately 4,807 meters above sea level. Would you like to check the elevation profile for a path around this area?


## Installation & Usage

To install and use the **Jawg Maps (Location & Routing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jawg-maps-location-routing](https://vinkius.com/mcp/jawg-maps-location-routing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
