# Nominatim MCP Server

Geocode addresses, reverse geocode coordinates and explore OpenStreetMap data — no API key required.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nominatim)

## Overview
**Category:** developer-tools
**Tools Count:** 5

## Description
Connect to **Nominatim** and search the world's most comprehensive open-source geographic database through natural conversation — no API key needed.

### What you can do

- **Address Search** — Find any place by name, address or type of place (restaurants, schools, hospitals)
- **Reverse Geocoding** — Convert GPS coordinates to human-readable addresses
- **OSM Lookup** — Look up detailed info for any OpenStreetMap object by its ID
- **Structured Addresses** — Get detailed address components (street, city, state, postal code, country)
- **Multi-language Names** — Retrieve place names in different languages
- **Bounding Boxes** — Get geographic boundaries for cities, countries and regions

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore geographic data from Claude, Cursor, or any MCP-compatible client

No API key required — completely free, powered by OpenStreetMap community data.

### Who is this for?

- **Developers** — geocode addresses and convert coordinates without paid geocoding services
- **Travelers** — find addresses and discover what's at any GPS coordinate
- **Researchers** — explore OpenStreetMap object details, administrative boundaries and place hierarchies
- **Data Analysts** — batch geocode addresses and extract structured location data


## Available Tools
- **get_details**: Returns the object's full name, display name, place rank, importance score, bounding box, parent place hierarchy, linked Wikipedia/Wikidata articles and optional extratags. OSM type: N (node), W (way), R (relation).

Get detailed info for an OSM object
- **lookup_osm**: IDs are formatted as "type{id}" where type is N (node), W (way) or R (relation). Multiple IDs are comma-separated. Returns the object's display name, coordinates, bounding box and properties.

Look up OSM objects by ID
- **reverse_geocode**: Returns the nearest address, city, state, country and other location details. Supports different zoom levels for varying detail granularity.

Convert coordinates to an address
- **search**: Returns results with coordinates, bounding box, display name, address components and OSM type/id. Supports structured searches with country codes and viewbox for region prioritization. Rate limited to 1 request/second.

Search for places by name or address
- **get_status**: Returns status message and response latency. Useful for verifying the service is operational before making other requests.

Get Nominatim server status


## Installation & Usage

To install and use the **Nominatim** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nominatim](https://vinkius.com/mcp/nominatim)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
