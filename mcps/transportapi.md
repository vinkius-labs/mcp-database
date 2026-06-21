# TransportAPI MCP Server

Access UK public transport data via TransportAPI — track buses and trains, plan journeys, check departures, and monitor service disruptions from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/transportapi)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Connect your **TransportAPI** UK public transport data platform to any AI agent and take full control of real-time bus and rail tracking, multimodal journey planning, and service disruption monitoring across Great Britain through natural conversation.

### What you can do

- **Real-Time Bus Tracking** — Check upcoming departures and arrivals at any UK bus stop with ETAs and delay indicators
- **Rail Services** — Monitor train arrivals, departures, and services at any UK rail station
- **Journey Planning** — Plan door-to-door multimodal trips combining bus, rail, tram, underground, walking, and cycling
- **Stop Discovery** — Search UK bus stops by name, address, or landmark with Naptan identifiers
- **Route Analysis** — Get train route information between any two UK rail stations with calling points
- **Service Updates** — Check real-time disruption alerts and operational notices across UK transport networks
- **Bus Timetables** — Access complete timetables for any UK bus line with weekday/weekend patterns
- **Station Information** — Get detailed UK rail station data including facilities, accessibility, and managing TOCs
- **Stop Details** — Retrieve comprehensive bus stop information with served lines and accessibility features

### How it works

1. Subscribe to this server
2. Enter your TransportAPI credentials (App ID and App Key from the developer portal)
3. Start tracking UK public transport from Claude, Cursor, or any MCP-compatible client

No more navigating multiple transport operator websites or manually parsing real-time data feeds. Your AI acts as a dedicated UK travel planner and transit operations analyst.

### Who is this for?

- **UK Commuters** — track buses and trains, plan journeys, and check disruptions before traveling
- **Tourists** — navigate UK public transport with multimodal journey planning and stop discovery
- **Transit Analysts** — research service patterns, station facilities, and operational performance
- **Travel Apps** — integrate real-time UK transit data into mobility and journey planning applications


## Available Tools
- **get_bus_arrivals**: Returns list of arriving services with line names and numbers, origins, scheduled and real-time arrival times (ETA), expected wait times, direction, operator details, and any delay indicators. Essential for passenger pickup coordination, arrival monitoring, and real-time arrival boards. AI agents use this when users ask "when is the next bus arriving at this stop", "show incoming buses at stop X", or need to track arriving bus services for passenger coordination.

Get real-time bus arrivals at a specific UK stop
- **get_bus_departures**: Returns list of departing services with line names and numbers, destinations, scheduled and real-time departure times (ETD), expected wait times, direction, operator details, and any service disruption notices. Covers all bus services across Great Britain including London Buses, Transport for Greater Manchester, West Midlands, and regional operators. Essential for passenger information displays, departure boards, journey planning, and real-time transit monitoring. AI agents should reference this when users ask "when is the next bus from this stop", "show departures from stop ID X", or need to monitor upcoming bus services at a known UK bus stop.

Get real-time bus departures from a specific stop in the UK
- **get_journey_plan**: Supports multimodal trips combining bus, rail, tram, underground (tube), walking, and cycling. Returns complete itinerary with departure and arrival times, total duration, number of changes, legs with mode details (line name, operator, vehicle type), intermediate stops/stations, walking distances, and real-time disruption information. Essential for travel planning, multimodal journey optimization, passenger information systems, and UK-wide mobility applications. AI agents should use this when users ask "how do I get from London Victoria to Heathrow Airport", "plan a journey from Manchester Piccadilly to Old Trafford", or need door-to-door trip planning across UK public transport.

Plan a multimodal journey between two UK locations
- **get_rail_arrivals**: Returns list of arriving services with train operating companies, origins, scheduled and real-time arrival times (ETA), platforms, expected delays, cancellation status, and service type information. Covers all National Rail services. Essential for passenger pickup coordination, arrival monitoring, station management, and real-time arrival boards. AI agents use this when users ask "what trains are arriving at Kings Cross", "show incoming trains at Manchester Piccadilly", or need to track arriving rail services.

Get real-time train arrivals at a specific UK rail station
- **get_rail_departures**: Returns list of departing services with train operating companies, destinations, scheduled and real-time departure times (ETD), platforms, expected delays, cancellation status, calling points, and service type (express, local, sleeper). Covers all National Rail services across Great Britain. Essential for departure boards, journey planning, station operations, and passenger information. AI agents should use this when users ask "what trains are leaving Paddington", "show departures from Birmingham New Street", or need comprehensive departure listings for a UK rail station.

Get real-time train departures from a specific UK rail station
- **get_rail_route**: Returns available services, journey duration, number of changes, calling points, train operating companies, typical frequency, and first/last service times. Essential for rail journey planning, route comparison, travel itinerary preparation, and understanding rail connectivity. AI agents should reference this when users ask "what is the train route from London to Manchester", "show rail connections between Edinburgh and Glasgow", or need to understand rail service options between two UK stations.

Get train route information between two UK rail stations
- **get_rail_services**: Returns services with train operating companies (TOCs), destinations, origins, scheduled times, platforms, service types (express, local, sleeper), and any disruption information. Covers National Rail services across Great Britain. Essential for station information displays, service monitoring, rail journey planning, and operational awareness. AI agents should reference this when users ask "what services call at Euston", "show all trains at Edinburgh Waverley", or need comprehensive service listings for a UK rail station.

Get all train services calling at a specific UK rail station
- **search_stops**: Returns matching stops with Naptan stop IDs, names, locations (latitude, longitude), served lines, localities, and stop types. Essential for stop discovery, journey planning interfaces, transit stop identification, and building location-based transit features. AI agents should use this when users ask "find the bus stop near Oxford Street", "search for stops called Piccadilly", or need to identify Naptan stop IDs for use in departure/arrival queries.

Search for UK bus stops by name, location, or landmark
- **get_station_info**: Returns station name, location (address, latitude, longitude), facilities (ticket office, ticket machines, waiting room, car park, cycle storage, WiFi, step-free access), staffing hours, managing train operating company, annual entry/exit statistics, and accessibility information. Essential for station planning, accessibility assessment, facility verification, and passenger information. AI agents should use this when users ask "tell me about Clapham Junction station", "does Euston have step-free access", or need detailed station metadata for UK rail journey planning.

Get detailed information about a specific UK rail station
- **get_stop_info**: Returns stop name, location (latitude, longitude, address, locality, landmark), common services, served lines, stop type (bus stop, bus station, coach station), accessibility features (wheelchair access, sheltered, seating), and operator information. Essential for stop identification, accessibility planning, transit network analysis, and passenger information. AI agents should use this when users ask "tell me about this bus stop", "what lines serve stop X", or need detailed stop metadata to contextualize transit queries.

Get detailed information about a specific UK bus stop
- **get_timetable**: Returns all scheduled services with departure times from origin through to terminus, stops served in sequence, journey duration variations by time of day, weekday/weekend/holiday service patterns, operator information, and any planned service changes. Essential for comprehensive schedule analysis, journey planning at specific times, service pattern research, and understanding bus frequency throughout the day. AI agents use this when users ask "show me the full timetable for bus route 73", "what times does the X59 run on Sundays", or need complete schedule data for a UK bus service.

Get full timetable for a specific UK bus line
- **get_updates**: Returns active alerts with affected lines, services, or operators, disruption descriptions, severity levels, expected duration, alternative route recommendations, and timestamps. Covers bus, rail, tram, and underground services across Great Britain. Essential for disruption awareness, passenger communication, journey reliability monitoring, and travel planning during service changes. AI agents should reference this when users ask "are there any disruptions on the Northern Line", "is there engineering work on Great Western Railway", or need to check service reliability before planning UK journeys.

Get real-time service updates and disruption alerts for UK transport


## Installation & Usage

To install and use the **TransportAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transportapi](https://vinkius.com/mcp/transportapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
