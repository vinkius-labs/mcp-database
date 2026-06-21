# LocationIQ (Geocoding & Maps) MCP Server

Build with location data via LocationIQ — geocode addresses, calculate routes, and perform reverse lookups.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/locationiq-geocoding-maps)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **LocationIQ** account to any AI agent and take full control of affordable geocoding, routing, and geospatial intelligence through natural conversation.

### What you can do

- **Geocoding & Search** — Convert address strings into precise GPS coordinates and use autocomplete to retrieve suggestions for partial location queries directly from your agent
- **Reverse Geocoding** — Convert latitude and longitude coordinates into human-readable addresses, including precise postal data and localized language translations
- **Advanced Routing** — Calculate optimal driving, walking, or cycling paths between multiple coordinates with support for OSRM-based navigation instructions
- **Distance Matrices** — Compute travel duration and distance tables between multiple origins and destinations to optimize logistics and delivery workflows
- **Road Snapping** — Perfectly align messy GPS signals to the exact street network using native snapping configurations for accurate fleet tracking
- **Geo-Fencing & Filtering** — Restrict searches within specific country ISO codes or geographic bounding boxes to ensure data relevancy and regional compliance

### How it works

1. Subscribe to this server
2. Enter your LocationIQ API Key
3. Start building location-aware applications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — integrate geocoding and routing services into AI agents and validate coordinate results through natural conversation
- **Logistics Managers** — calculate optimal routes and distance matrices for delivery fleets without manual GIS software
- **Data Analysts** — clean and enrich datasets with precise geolocation and postal address metadata efficiently


## Available Tools
- **search_autocomplete**: php` tracking prefix queries and parsing city datasets quickly.

Retrieve autosuggest lists for partial location search queries
- **check_account_balance**: php` verifying explicitly how many OpenStreetMap queries remain for the Tenant API Key.

Validate current LocationIQ account balance and remaining requests
- **calculate_directions**: Calculate optimal driving, walking, or cycling route between coordinates
- **calculate_distance_matrix**: Calculate travel duration table crossing multiple coordinate sources and destinations
- **snap_nearest_roads**: Snap a coordinate perfectly to the exact street network
- **reverse_geocode**: php` pulling standard Place objects formatting explicit postal addresses over GPS positions.

Convert latitude and longitude coordinates into a human-readable address
- **reverse_language_bias**: Reverse Geocode lat/lon mapping translations inside specific native language tags
- **search_geocode**: php` mapping address strings into specific OpenStreetMap coordinates securely.

Convert an address string into latitude and longitude coordinates
- **search_bounding_box**: Search explicitly bounded within a geographical map rectangle
- **search_country_filter**: Search address coordinates forced within explicit Country codes


## Installation & Usage

To install and use the **LocationIQ (Geocoding & Maps)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/locationiq-geocoding-maps](https://vinkius.com/mcp/locationiq-geocoding-maps)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
