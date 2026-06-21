# OpenRouteService MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openrouteservice)
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


## Available Tools (10)
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


## ❓ FAQ

**Q: Is the OpenRouteService API free?**
Yes. ORS offers a free Standard plan with generous daily limits for all services (directions, isochrones, matrix, geocoding, and optimization). No credit card required. Higher rate limits are available through the Collaborative plan for non-profits, academics, and government organizations.

**Q: What routing profiles are supported?**
ORS supports driving-car, driving-hgv (heavy goods vehicles), cycling-regular, cycling-road, cycling-mountain, cycling-electric, foot-walking, foot-hiking, and wheelchair. Each profile optimizes routes based on road network restrictions specific to that transportation mode.

**Q: Can I solve vehicle routing problems with time windows and capacity constraints?**
Yes. The VRP optimization tool uses the VROOM solver. Define jobs with locations, service times, and time windows, then define vehicles with start/end locations, capacities, and operating hours. The solver returns optimized assignments and routes for your entire fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openrouteservice](https://vinkius.com/mcp/openrouteservice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenRouteService** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openrouteservice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenRouteService** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openrouteservice": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
