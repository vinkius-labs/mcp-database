# Trimble MCP Server

Equip your AI agent with enterprise-grade truck routing, commercial geocoding, and advanced toll cost logistics algorithms.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/trimble)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your AI agent exclusively to your **Trimble PC*MILER** logistics infrastructure. Elevate your transportation operations replacing disjointed navigation screens. Communicate organically to your agent to dictate exact vehicle dimensions to avoid tight bridges, compile meticulous state-by-state fuel mileage reports, or estimate holistic transit budgets using precise industrial coordinates.

### What you can do

- **Heavy Routing Limits** — Command a route trace bypassing commercial hazard zones using variables like actual truck dimensions (height, weight) directly in conversation
- **Toll Estimation** — Ping exactly how much a full route will impact your budget by breaking down both cash and electronic toll values mathematically
- **State Mileage Reporting** — Generate automatic fuel-tax (IFTA) summaries calculating exact penetration mileage crossed inside individual states
- **Logistics Forensics** — Interrogate geographical locations using structured isochrone grids (predicting max travel based on an hour limit) or matrix origins
- **Spatial Exclusions** — Trace itineraries avoiding strictly designated public roads and restricting expressways in the blink of an eye

### How it works

1. Provision this connector inside your central Vinkius matrix
2. Inject your certified Trimble Developer API Key
3. Start addressing fleet transit instructions directly mapping routes over any environment

### Who is this for?

- **Fleet Operations Managers** — Oversee large transport deployments bypassing hazards evaluating toll expenditures across specific trips in milliseconds
- **Logistical Data Scientists** — Plot broad origins-destinations distance matrices interacting solely through terminal queries over heavy machinery requirements
- **Dispatch Analysts** — Investigate delivery reach by requesting an active 'time shed' (isochrone) boundary estimating limits for rush transit manually


## Available Tools
- **calculate_driving_isochrone**: Provide center coordinates and time in minutes.

Calculates the reachable area within a specific time limit from a center point
- **calculate_matrix_routing**: Provide arrays of lon,lat points.

Calculates distances and travel times between multiple origins and destinations
- **calculate_state_mileage**: Calculates mileage broken down by US state or province for a given route
- **calculate_trip_tolls**: Returns cash and electronic toll fees in USD.

Estimates the total toll costs for a specific truck route
- **calculate_truck_route**: Returns distance, time, and routing polyline.

Calculates a truck-compliant route between multiple stops using Trimble PC*MILER
- **get_truck_directions**: Considers bridge heights, HazMat restrictions, and weight limits.

Retrieves turn-by-turn driving directions for a truck route
- **route_avoiding_roads**: Calculates a route that explicitly avoids certain roads or expressways
- **route_by_vehicle_size**: Provide vehicle height in inches and weight in lbs.

Calculates a truck route using specific vehicle dimensions
- **search_trimble_address**: Searches for locations and commercial addresses in the Trimble database
- **reverse_geocode**: Converts geographic coordinates into the nearest commercial address


## Installation & Usage

To install and use the **Trimble** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/trimble](https://vinkius.com/mcp/trimble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
