# TfL MCP Server

Access London transport data via TfL — track tube and bus arrivals, plan journeys, check line status, and find bike points from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tfl)

## Overview
**Category:** government-public-data
**Tools Count:** 12

## Description
Connect your **TfL Unified API** London public transport data platform to any AI agent and take full control of real-time Tube and bus tracking, multimodal journey planning, line status monitoring, and Santander Cycles availability through natural conversation.

### What you can do

- **Real-Time Arrivals** — Get live arrival predictions for any Tube station, bus stop, DLR, Overground, Elizabeth line, tram, river, or cable-car stop
- **Stop Point Search** — Find any TfL stop point by station name, street, or landmark across all transport modes
- **Line Status** — Check current service status for all Tube lines, bus routes, DLR, Overground, Elizabeth line, and more
- **Journey Planning** — Plan door-to-door multimodal trips combining Tube, bus, DLR, Overground, Elizabeth line, tram, walking, and cycling
- **Stop Details** — Get comprehensive station information including accessibility, fare zones, and step-free access
- **Santander Cycles** — Browse all bike docking stations with real-time availability (bikes and empty docks)
- **Road Status** — Monitor London road conditions, closures, and disruptions for driving planning
- **Place Search** — Discover places and points of interest across London by category
- **Transport Modes** — Explore all available transport modes in the TfL network
- **Vehicle Compliance** — Check ULEZ and Congestion Charge compliance for registered vehicles

### How it works

1. Subscribe to this server
2. Enter your TfL Application ID and Application Key (free from the developer portal)
3. Start tracking London transport from Claude, Cursor, or any MCP-compatible client

No more navigating multiple TfL apps or manually checking arrival boards. Your AI acts as a dedicated London transport analyst and journey planning assistant.

### Who is this for?

- **London Commuters** — track Tube and bus arrivals, check line status, and plan daily commutes
- **Tourists** — navigate London with multimodal journey planning and station discovery
- **Cyclists** — check Santander Cycles availability at docking stations across the city
- **Drivers** — monitor road status, disruptions, and ULEZ compliance before driving in London


## Available Tools
- **get_arrivals**: g., 940GZZLUSCL for Oxford Circus Underground, or 490007653 for a bus stop). Returns predicted arrival times, line names, destination stations, time to station in minutes, vehicle IDs, expected arrival timestamps, and service types (tube, bus, dlr, elizabeth-line, overground, tram, river, cable-car). Essential for real-time arrival awareness, passenger waiting time estimation, trip timing, and connection coordination across the entire London transport network. AI agents should reference this when users ask "when is the next Northern Line train at Bank", "show upcoming buses at stop 490007653", or need real-time arrival predictions for any TfL stop point. Stop IDs can be found using search_stop_point.

Get real-time arrival predictions for a specific TfL stop point
- **get_bike_point**: Returns dock ID, common name, precise location (latitude, longitude, address), total capacity, current available bikes, current empty docks, installation date, last update timestamp, and operational status. Essential for dock-level bike availability checks, capacity planning, and real-time bike-sharing awareness for specific docking stations. AI agents should use this when users ask "how many bikes are at dock BikePoints_1234", "tell me about the docking station at Hyde Park Corner", or need specific docking station details for bike hire planning.

Get detailed information about a specific Santander Cycles docking station
- **get_bike_points**: Returns docking station IDs, common names, geographic coordinates, total bike capacity, number of available bikes, number of empty docks, installation date, and operational status. Covers thousands of docking stations across central London and expanding into outer boroughs. Essential for bike hire planning, dock availability awareness, cycle route planning, and understanding London's bike-sharing network coverage. AI agents should reference this when users ask "where are the nearest bike docking stations", "how many bikes are available at this dock", or need to identify bike hire options for last-mile connectivity.

List all Santander Cycles (bike hire) docking stations across London
- **get_journey**: Returns multiple route options combining tube, bus, dlr, overground, elizabeth-line, tram, river, walking, and cycling. Each route includes total duration, walking distance, number of interchanges, fare estimates, CO2 savings, and detailed leg-by-leg instructions with line names, directions, station sequences, and departure/arrival times. Essential for multimodal trip planning, route comparison, accessibility-aware journey selection, and passenger information. AI agents should use this when users ask "how do I get from Paddington to Greenwich", "plan a journey from Heathrow to Tower Bridge", or need door-to-door trip planning across London's transport network.

Plan a journey between two locations using TfL transport modes
- **get_line_status**: Returns line IDs, line names, status severity (Good Service, Minor Delays, Severe Delays, Part Suspended, Suspended, Planned Work, Special Service), status descriptions, reason codes, and disruption details. Can query all lines system-wide or filter by specific modes (tube, bus, dlr, overground, tram, river, cable-car, elizabeth-line, national-rail). Essential for service disruption awareness, alternative route planning, passenger communication, and understanding overall TfL reliability. AI agents should reference this when users ask "is the Victoria Line running normally", "what is the status of the Overground", or need to check service reliability before planning London journeys.

Get current service status for TfL lines, optionally filtered by mode
- **get_modes**: Returns modes including tube, bus, dlr, overground, elizabeth-line, tram, river, cable-car, national-rail, and walking. Essential for understanding the scope of TfL's multimodal network, mode identification for filtered queries, and transport network analysis. AI agents should reference this when users ask "what transport modes does TfL cover", "list all available modes", or need to understand the full range of London transport options before planning journeys.

List all available transport modes in the TfL network
- **get_place_search**: Returns place IDs, names, categories, geographic coordinates, address information, and related links. Can optionally filter by place type (e.g., "TubeStation", "BusStation", "Park", "Museum", "Hospital"). Essential for place discovery, tourist planning, accessibility research, and understanding London's infrastructure. AI agents should use this when users ask "find parks near Westminster", "search for museums in South Bank", or need to identify places and points of interest for comprehensive London trip planning.

Search for places and points of interest across London
- **get_road_disruptions**: Returns disruption descriptions, affected road segments, cause types (roadworks, incidents, events, utility works), start and end dates, severity levels, and alternative route recommendations. Can query all disruptions system-wide or filter by specific road. Essential for driving disruption awareness, alternative route planning, delivery logistics, and understanding road reliability. AI agents should reference this when users ask "are there any roadworks on the A4", "what disruptions affect my drive to Heathrow", or need to check road conditions before planning driving journeys in London.

Get current road disruptions and closures across London
- **get_road_status**: Returns road IDs, road names, status descriptions, corridor details, and operational information. Can query all roads system-wide or filter by a specific road ID (e.g., "A1", "A40", "A205" South Circular). Essential for driving route planning, road closure awareness, understanding London road network conditions, and commuter driving decisions. AI agents should use this when users ask "what is the status of the A40", "are there any road closures on the North Circular", or need to check road conditions before driving journeys in London.

Get current status of London roads, optionally filtered by specific road
- **search_stop_point**: Returns matching stop points with their IDs, common names, modes served (tube, bus, dlr, overground, tram, river, cable-car, elizabeth-line), geographic coordinates (lat/lon), and station hierarchy information. Can optionally filter by transport mode. Essential for stop discovery, journey planning interfaces, stop identification, and building location-based transit features. AI agents should use this when users ask "find the tube station near Covent Garden", "search for stops called Victoria", or need to identify stop IDs for use in arrival queries.

Search for TfL stop points by name or location
- **get_stop_point_details**: Returns stop ID, common name, station type, modes served, geographic coordinates, address, accessibility information (step-free access, lift availability), fare zone, hub station affiliations, and parent/child station relationships. Essential for stop identification, accessibility planning, fare zone awareness, station navigation, and understanding station hierarchy in the TfL network. AI agents should use this when users ask "tell me about King's Cross station", "is this station step-free", or need detailed stop metadata to contextualise transit queries.

Get detailed information about a specific TfL stop point
- **get_vehicle_details**: Returns vehicle registration, make, model, compliance status, charge exemptions, and registration dates. Essential for London driving compliance checks, ULEZ awareness, congestion charge planning, and vehicle registration verification. AI agents should use this when users ask "check if vehicle AB12 CDE is ULEZ compliant", "is my car exempt from Congestion Charge", or need to verify vehicle compliance before driving in central London.

Get vehicle details for a registered vehicle in London (ULEZ/congestion charge)


## Installation & Usage

To install and use the **TfL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tfl](https://vinkius.com/mcp/tfl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
