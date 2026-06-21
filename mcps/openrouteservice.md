# OpenRouteService MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openrouteservice)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openrouteservice-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openrouteservice-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Plan routes and analyze spatial data via OpenRouteService — calculate directions, isochrones, distance matrices, VRP optimization, and geocoding from any AI agent.

## Description
Unlock the full power of **OpenRouteService** from a single conversation. Calculate driving routes, generate reachability maps, solve vehicle routing problems, and geocode addresses — all backed by OpenStreetMap data.

### What you can do

- **Directions** — Calculate optimal routes between multiple waypoints for car, bicycle, or pedestrian profiles with distance and duration
- **Isochrones** — Generate reachability polygons showing areas accessible within a given time or distance from any point
- **Distance Matrix** — Compute M×N duration and distance matrices between multiple origins and destinations
- **VRP Optimization** — Solve multi-vehicle routing problems with jobs, vehicles, and capacity constraints using the VROOM solver
- **Geocoding** — Forward and reverse geocode addresses using Pelias, with country boundary filters
- **GPS Snap** — Clean noisy GPS traces by snapping coordinates to the nearest road segment
- **Elevation** — Get altitude data for coordinate sequences using the elevation API

### How it works

1. Subscribe to this server
2. Enter your OpenRouteService API Key
3. Start planning routes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics teams** — optimize multi-stop delivery routes and estimate travel times between warehouses and customers
- **Urban planners** — analyze accessibility with isochrone maps showing 5/10/15-minute reachability zones
- **Field service managers** — plan technician routes solving vehicle routing problems with capacity and time window constraints


## Available Tools
- **calculate_directions**: Identify precise active arrays spanning native Road network points
- **get_elevation_line**: Provision a highly-available JSON Payload parsing accessible Altitude lines
- **search_country_boundary**: country` fetching strings rigidly ignoring maps spanning outside target ISO boundaries.

Irreversibly vaporize explicit validations extracting local search filters
- **reverse_geocode**: Perform structural extraction of properties driving active OSM boundaries
- **geocode_search**: Identify bounded routing spaces inside the Headless OpenRouteService
- **calculate_isochrones**: Inspect deep internal arrays mitigating specific Reachability lines
- **calculate_matrix**: Enumerate explicitly attached structured rules exporting active M * N logs
- **check_optimization_status**: Retrieve explicit Cloud logging tracing explicit Optimization jobs
- **solve_vrp_optimization**: Dispatch an automated validation check routing explicit VROOM solvers
- **snap_gps_to_road**: Retrieve the exact structural matching verifying Map snapping limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenRouteService** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a driving route from Berlin to Munich with estimated time."

**🤖 AI Agent:**
> Route calculated (driving-car): Berlin → Munich. Distance: 585 km. Duration: 5h 42min. Route passes through Leipzig and Nuremberg. 2 toll sections detected. Want me to generate an isochrone from the destination or calculate the return route?

---

**👤 You:**
> "Show me all areas reachable within 15 minutes by car from Times Square."

**🤖 AI Agent:**
> Isochrone generated for Times Square (40.7580, -73.9855) with 15-minute driving range. The polygon covers approximately 12 km² including Midtown, Upper East/West Side, Chelsea, and parts of the East Village. GeoJSON available. Want me to also generate 5 and 10-minute isochrones for comparison?

---

**👤 You:**
> "Calculate the distance matrix between our 3 warehouses and 5 customer locations."

**🤖 AI Agent:**
> 3×5 distance matrix computed (driving-car). Shortest pair: Warehouse B → Customer 3 (8.2 km, 14 min). Longest pair: Warehouse A → Customer 5 (47.1 km, 52 min). Average delivery time across all pairs: 28 min. Want me to run VRP optimization to assign optimal warehouse-customer pairs?


## Installation & Usage

To install and use the **OpenRouteService** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openrouteservice](https://vinkius.com/mcp/openrouteservice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
