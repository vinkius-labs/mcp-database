# SafeGraph MCP Server

Integrate SafeGraph's premier geospatial dataset into your AI. Discover detailed POIs, analyze foot traffic patterns, and process precise building geometries seamlessly from conversational prompts.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/safegraph)

## Overview
**Category:** data-analytics
**Tools Count:** 10

## Description
Empower your AI with direct connectivity to **SafeGraph**, the foundational geospatial and mobility dataset trusted by top analytics and enterprise organizations globally. This robust integration converts your AI into an expert geographical analyst capable of retrieving precise intelligence surrounding global structures, Points of Interest (POIs), and detailed patterns—all without touching complex database pipelines.

### What you can do

- **Rich Context on POIs** — Fetch exhaustive lists of businesses or brands within targeted radii (`search_distance_radius`, `search_brand_places`). You can also slice the results according to their designated NAICS industry codes region-to-region (`search_industry_naics`).
- **Deep Geospatial Footprints** — Look up exact WKT polygons for targeted individual buildings (`lookup_building_geometry`) or identify everything bounded inside designated custom city borders (`search_wkt_polygon`). Understand structural hierarchies immediately by querying parent containers like malls or industrial complexes (`lookup_parent_polygon`).
- **Pedestrian and Mobility Insights** — Audit recent visit metrics, dwell times, and absolute foot traffic measurements attached to individual structures leveraging historical aggregation points (`lookup_place_patterns`).
- **Native GraphQL Exploration** — Pass perfectly structured GraphQL queries straight to the root mapping infrastructure for fully-unlocked edge cases (`graphql_raw_query`). Request and resolve bulk Placekeys efficiently on demand (`batch_lookup_placekeys`).

### How it works

1. Install this SafeGraph mapping block into your AI workspace.
2. Sign into the SafeGraph Dashboard environment.
3. Request or generate a valid GraphQL API Key within your workspace settings.
4. Input that key securely. Chat instantly: "Find all coffee shop POIs located within a 500-meter radius around longitude -122.33, latitude 47.60."


## Available Tools
- **batch_lookup_placekeys**: Provide them as a JSON array.

Performs multiple Placekey lookups in a single request
- **graphql_raw_query**: Provide the query string and optional variables.

Executes a raw GraphQL query against the SafeGraph API
- **lookup_building_geometry**: Retrieves the building footprint (polygon) for a specific Placekey
- **lookup_parent_polygon**: Identifies the parent Placekey for a location (e.g., mall or airport)
- **lookup_place_patterns**: Retrieves historical foot traffic patterns for a specific Placekey
- **lookup_placekey**: Retrieves detailed attributes for a specific location by its Placekey
- **search_brand_places**: g., "Starbucks") in a specific city.

Searches for locations of a specific brand in a city
- **search_distance_radius**: Specify lat, lon, and radius in meters.

Searches for places within a specific radius from a point
- **search_industry_naics**: Searches for places by NAICS industry code and region
- **search_wkt_polygon**: Finds all places within a specific geometric polygon (WKT)


## Installation & Usage

To install and use the **SafeGraph** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/safegraph](https://vinkius.com/mcp/safegraph)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
