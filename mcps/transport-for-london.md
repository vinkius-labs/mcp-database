# Transport for London MCP Server

Get live tube status, bus arrivals, journey planning, road disruptions and bike point data across London.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/transport-for-london)

## Overview
**Category:** productivity
**Tools Count:** 11

## Description
Connect to **Transport for London (TfL)** and access real-time London transit data through natural conversation — no API key needed.

### What you can do

- **Tube Status** — Check real-time status of all Underground lines (Good Service, Minor/Severe Delays, Suspended)
- **Line Details** — Get detailed info about any tube, overground, DLR, Elizabeth line or tram route
- **Bus Arrivals** — Get live bus arrival predictions for any stop
- **Journey Planning** — Plan journeys between any two London locations with step-by-step directions
- **Road Status** — Check major road status and disruptions across London
- **Bike Points** — Find Santander Cycle docking stations with bike and dock availability
- **Stop Search** — Search for bus stops, tube stations and river piers by name

### How it works

1. Subscribe to this server
2. No API key needed — TfL API is free and open
3. Start exploring London transit data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **London Commuters** — check tube status, plan journeys and find bus arrivals in real-time
- **Tourists** — navigate London's transport system with live arrival data and journey planning
- **Developers** — integrate TfL transit data into apps and travel tools


## Available Tools
- **get_arrivals**: Returns predicted arrival times, destination, line number, vehicle ID and expected time to station. Use the stop point ID (e.g. "490009056W") from search_stop.

Get live arrival predictions for a bus stop
- **get_bike_point_detail**: Get detailed info for a specific bike docking station
- **get_bike_points**: Returns bike availability, dock availability, station locations and status. Useful for finding nearby bikes for cycling journeys.

Search for Santander Cycle (Boris Bike) docking stations
- **get_journey**: Returns multiple route options with estimated duration, walking distance, fare cost, number of changes and step-by-step directions. Input locations can be station names, addresses or postcodes.

Plan a journey between two points in London
- **get_line_detail**: Supports tube, overground, DLR, Elizabeth line, tram and river bus lines.

Get detailed information about a specific TfL line
- **get_line_routes**: Returns the ordered list of stations the line serves. Useful for understanding the full journey path of a tube line.

Get the route sequence for a TfL line
- **get_line_status**: Shows whether each line has Good Service, Minor Delays, Severe Delays, or is Suspended/Part Suspended. If no line IDs specified, returns all tube lines. Use line_ids to check specific lines (comma-separated, e.g. "central,victoria,northern").

Get real-time status for TfL tube lines
- **get_road_disruptions**: Returns disruption details with severity, location, cause and estimated clearance times.

Get current road disruptions in London
- **get_road_status**: Shows whether roads have Good, Minor or Severe congestion.

Get status of London major roads
- **get_stop_details**: Useful for identifying the correct stop ID for arrival queries.

Get details for a specific bus stop or station
- **search_stop**: Returns matching stops with their IDs, locations, modes and routes. Use the returned IDs with get_arrivals or get_stop_details.

Search for bus stops and stations by name


## Installation & Usage

To install and use the **Transport for London** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transport-for-london](https://vinkius.com/mcp/transport-for-london)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
