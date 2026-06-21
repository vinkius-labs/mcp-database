# TripGo MCP Server

AI multimodal transit: plan trips, track vehicles, and check schedules via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tripgo)

## Overview
**Category:** travel-hospitality
**Tools Count:** 9

## Description
### What you can do

Connect AI agents to the TripGo platform for intelligent multimodal journey planning:

- **Plan trips** combining bus, train, subway, tram, ferry, walking, and cycling
- **Find nearby transit stops** by GPS coordinates with distance and route info
- **Search stops by name** or address for precise location discovery
- **Get real-time departures and arrivals** with live delay estimates
- **Track vehicle positions** on the map with real-time GPS data
- **Review route information** including all stops and agency details
- **Check stop details** with accessibility and amenity information
- **Access global regions** covering major cities worldwide

### How it works

1. **Get your TripGo API key** from developer.tripgo.com (free tier available)
2. **Ask your AI agent** to plan trips, check schedules, or track vehicles
3. **Natural language commands** replace complex transit app navigation
4. **Multimodal planning** combining public transit with active transportation modes

### Who is this for?

Perfect for **urban commuters**, **multimodal travelers**, **cyclists**, **pedestrians**, **transit riders**, **accessibility planners**, and **eco-conscious citizens**. Let AI agents find optimal routes combining buses, trains, bikes, and walking. Ideal for daily commuters who want to compare route options, check real-time departures, track incoming vehicles, and plan sustainable journeys without car dependency.


## Available Tools
- **get_arrivals**: Returns route names, origins, scheduled vs estimated arrival times, and delays. Use this to track incoming vehicles. Requires stop ID.

Get upcoming arrivals to a transit stop
- **get_departures**: Returns route names, destinations, scheduled vs estimated departure times, and delays. Use this to check when your next ride arrives. Requires stop ID.

Get upcoming departures from a transit stop
- **get_nearby_stops**: Returns stop IDs, names, coordinates, routes serving each stop, and distance from search point. Use this to find nearest transit options before planning trips.

Find transit stops near a GPS coordinate
- **get_regions**: Each region has an ID, name, and coverage area. Use this first to verify your city is covered before planning trips. Supports major cities across North America, Europe, Australia, and Asia.

List all available transit regions supported by TripGo
- **get_route_info**: Requires route ID. Use this to understand route coverage before planning trips.

Get information about a specific transit route
- **get_stop_details**: Requires stop ID from nearby stops or search results. Use this to review stop facilities before waiting there.

Get detailed information about a specific transit stop
- **get_vehicle_positions**: Optionally filter by route ID. Use this for real-time tracking of vehicles on the map.

Get real-time vehicle positions for transit vehicles
- **plan_trip**: Combines public transport (bus, train, subway, tram, ferry) with walking and cycling. Returns multiple trip options with departure/arrival times, duration, number of transfers, and step-by-step instructions. Optionally specify travel time and preferred transport modes.

Plan a multimodal trip between two coordinates
- **search_stops**: g., "Times Square", "Main St & 5th Ave"). Returns matching stops with IDs, names, coordinates, routes, and relevance scores. Use this when you know the stop name or intersection but not exact coordinates.

Search for transit stops by name or address


## Installation & Usage

To install and use the **TripGo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tripgo](https://vinkius.com/mcp/tripgo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
