# TomTom MCP Server

Equip your AI agent with global mapping, routing, and real-time traffic capabilities powered by TomTom.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tomtom)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **TomTom** API account directly to any AI agent to unlock enterprise-grade geospatial and logistical capabilities native to your platform. Convert complex addresses instantly, evaluate driving routes based on exact origin and destination coordinates, and visualize live traffic blocks directly through chat queries.

### What you can do

- **Precision Geocoding** — Process any physical address string into absolute geographic latitude/longitude coordinates using fuzzy logic or structured fields, as well as reversing coordinates back to plain street names
- **Route Computation** — Calculate the exact travel time, polyline geometry, and distance for a trip between two precise coordinates
- **Real-Time Traffic** — Map traffic incidents (accidents, constructions, jams) constrained within a bounding box, or survey the traffic flow speed of a particular avenue segment
- **Poi Discovery** — Find global Points of Interest based on categories (e.g., hospitals, fuel) and retrieve rich contact metadata or opening hours for specific locations
- **Travel Boundaries** — Calculate reachable ranges (polygonal limits) to understand exactly how far your fleet or agents can travel within a set time budget

### How it works

1. Add this marketplace component to your workflow
2. Open the TomTom Developer Portal and produce a secure API token
3. Plug the key above, and start interrogating global geography immediately

### Who is this for?

- **Fleet Managers** — Ensure continuous auditing of road incidents and calculate travel time differences organically
- **Logistics Engineers** — Implement and test route shedding, time boundaries, and flow calculations locally
- **App Developers** — Programmatically pull local Points of Interest strings and contact numbers directly into their coding setup


## Available Tools
- **calculate_reachable_range**: Provide center coordinates and a time budget in seconds.

Calculates an area reachable within a specific time or distance budget
- **calculate_route**: Returns the route polyline and a summary.

Calculates a route and travel time between two points
- **search_poi_by_category**: Provide a category name and a center coordinate.

Searches for points of interest (POIs) near a location by category (e.g., gas stations, hospitals)
- **fuzzy_geocoding**: Converts a physical address string into geographic coordinates using fuzzy matching
- **get_poi_details**: Retrieves rich metadata for a specific point of interest ID
- **get_traffic_incidents**: Provide min/max lat/lon coordinates.

Retrieves real-time traffic incident details within a bounding box
- **get_traffic_flow_segment**: Provide center coordinates.

Retrieves the traffic flow speed and quality for a specific road segment
- **reverse_geocoding**: Converts geographic coordinates into a physical address
- **autocomplete_place_search**: Provide a partial string and optional bias coordinates.

Provides predictive location suggestions based on partial input
- **structured_geocoding**: Provide parameters like countryCode and postalCode.

Performs geocoding using explicit address components (e.g., street, city, zip)


## Installation & Usage

To install and use the **TomTom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tomtom](https://vinkius.com/mcp/tomtom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
