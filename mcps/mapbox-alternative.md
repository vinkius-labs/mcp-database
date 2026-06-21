# Mapbox MCP Server

Integrate Mapbox mapping and location services into your AI agent—access vector/raster tiles, static images, directions, and manage datasets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mapbox-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 27

## Description
Connect your **Mapbox** account to any AI agent to leverage powerful geospatial capabilities through natural language.

### What you can do

- **Maps & Tiles** — Retrieve vector and raster tiles or generate standalone static map images for specific coordinates and styles.
- **Navigation & Routing** — Calculate optimal routes with turn-by-turn instructions and travel time matrices between multiple locations.
- **Dataset Management** — List, retrieve, and update features within your Mapbox datasets directly from the conversation.
- **Tileset Publishing** — Create and publish tileset sources using the Mapbox Tiling Service (MTS) for custom map layers.
- **Spatial Queries** — Use Tilequery to retrieve detailed data about specific features at any given longitude and latitude.

### How it works

1. Subscribe to this server
2. Enter your Mapbox Access Token (Public or Secret)
3. Start querying maps, directions, and geospatial data from Claude, Cursor, or any MCP client

### Who is this for?

- **GIS Specialists & Developers** — quickly inspect dataset features and tileset statuses without leaving the terminal or editor.
- **Logistics Managers** — calculate routes and travel matrices to optimize fleet movements via simple AI prompts.
- **Data Analysts** — perform spatial queries and retrieve feature metadata for geographic research and reporting.


## Available Tools
- **geocode_reverse**: Reverse geocoding (v6)
- **get_dataset_feature**: Retrieve a specific feature from a dataset
- **get_directions**: Calculate optimal routes and turn-by-turn instructions
- **get_feedback**: Get user feedback
- **get_isochrone**: Computes reachable areas within a specified time or distance
- **get_map_matching**: Snaps fuzzy GPS traces to the road network
- **get_matrix**: Returns travel times or distances between many points
- **get_optimization**: Retrieve a previously submitted optimization solution
- **get_raster_tile**: png, .jpg, .webp, .grid.json) from a Mapbox-hosted tileset.

Get a raster tile from Mapbox
- **create_tileset_source**: Create a Mapbox Tiling Service (MTS) source
- **create_token**: Create a new access token
- **delete_token**: Delete an access token
- **geocode_batch**: Batch geocoding (v6)
- **geocode_forward**: Forward geocoding (v6)
- **get_static_image**: Get a static map image
- **get_tilequery**: Retrieve data about specific features from tilesets at a point
- **get_vector_tile**: mvt or .vector.pbf) from a Mapbox-hosted tileset.

Get a vector tile from Mapbox
- **list_datasets**: List Mapbox datasets for a user
- **list_tokens**: List access tokens for a user
- **publish_tileset**: Publish a Mapbox Tiling Service (MTS) tileset
- **searchbox_forward**: Forward search using the Search Box API
- **searchbox_retrieve**: Retrieve full details for a searchbox suggestion
- **searchbox_reverse**: Reverse search using the Search Box API
- **searchbox_suggest**: Interactive location search with autocomplete
- **submit_feedback**: Submit user feedback
- **submit_optimization**: Solves the Traveling Salesperson Problem for fleet routing
- **update_dataset_feature**: Update a specific feature in a dataset


## Installation & Usage

To install and use the **Mapbox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapbox-alternative](https://vinkius.com/mcp/mapbox-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
