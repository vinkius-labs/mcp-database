# TIGER/Line Geocoder (Census) MCP Server

Access official US Census Bureau geocoding services to convert addresses into coordinates and detailed census geography data.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tigerline-geocoder-census)

## Overview
**Category:** industry-titans
**Tools Count:** 8

## Description
Connect to the **US Census Bureau TIGER/Line Geocoder** to transform location data into actionable geographic insights directly within your AI agent.

### What you can do

- **Address Geocoding** — Convert single-line or structured addresses (street, city, state, zip) into precise latitude and longitude coordinates.
- **Census Geographies** — Retrieve high-resolution census data including tracts, blocks, and tribal areas for any location.
- **Puerto Rico Support** — Specialized geocoding for Puerto Rico addresses, including Urbanization and Municipio parameters.
- **Reverse Geocoding** — Submit coordinates to identify the exact census boundaries and administrative layers they fall within.
- **Batch Processing** — Process up to 10,000 addresses at once via CSV data for large-scale data analysis.
- **Benchmark Management** — List and select specific Census benchmarks and vintages to ensure data consistency across different time periods.

### How it works

1. Subscribe to this server
2. The service uses the public Census Bureau API (no complex registration required)
3. Start querying US geographic data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — automate the mapping of addresses to census tracts for demographic analysis.
- **Urban Planners** — quickly identify administrative boundaries and census blocks for infrastructure projects.
- **Logistics Teams** — validate US addresses and normalize geographic data for routing and delivery.


## Available Tools
- **batch_geocode_address**: Format: Unique ID, Street address, City, State, ZIP

Batch geocode up to 10,000 addresses
- **batch_geocode_coordinates**: Format: Unique ID, Longitude (X), Latitude (Y)

Batch lookup census geographies for coordinates
- **list_benchmarks**: g., Public_AR_Current) and their IDs.

List available Census Geocoder benchmarks
- **geocode_address_pr**: Geocode a structured Puerto Rico address
- **geocode_address**: Geocode a structured address
- **geocode_coordinates**: ) for a specific latitude and longitude.

Lookup census geographies for coordinates
- **geocode_oneline**: Geocode a single line address
- **list_vintages**: List available Census Geocoder vintages for a benchmark


## Installation & Usage

To install and use the **TIGER/Line Geocoder (Census)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tigerline-geocoder-census](https://vinkius.com/mcp/tigerline-geocoder-census)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
