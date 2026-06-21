# Lyko MCP Server

Access European public transit via Lyko — plan intermodal trips, check departures, search stops, and monitor transit operators from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lyko)

## Overview
**Category:** travel-hospitality
**Tools Count:** 12

## Description
Connect your **Lyko Transit API** mobility platform to any AI agent and take full control of European public transit planning, real-time departure monitoring, and multimodal journey optimization through natural conversation.

### What you can do

- **Trip Planning** — Plan door-to-door intermodal journeys combining buses, trains, subways, trams, ferries, bike-sharing, and walking
- **Real-Time Departures** — Check upcoming departures at any transit stop with ETAs, platforms, and delay indicators
- **Arrival Tracking** — Monitor incoming services for passenger pickup and connection coordination
- **Stop Discovery** — Search transit stops by name, address, or landmark across 300+ European operators
- **Nearby Stops** — Find all transit stops near any geographic location with distance calculations
- **Stop Details** — Get comprehensive stop information including served lines, accessibility, and amenities
- **Line Information** — Research transit lines with operator details, service hours, and route characteristics
- **Line Routes** — View complete stop sequences and route patterns for any transit line
- **Operator Directory** — Browse 300+ transit operators across Europe with coverage areas and service modes
- **Network Status** — Check service disruptions, planned works, strikes, and delay alerts for any operator
- **GTFS Feeds** — Access raw GTFS transit data for offline analysis and academic research
- **Trip Booking** — Book train tickets, bus passes, bike rentals, and other mobility services through Lyko Book

### How it works

1. Subscribe to this server
2. Enter your Lyko API key (from the Developer Portal)
3. Start planning European transit journeys from Claude, Cursor, or any MCP-compatible client

No more navigating multiple transit operator websites or manually parsing schedule data. Your AI acts as a dedicated European travel planner and transit operations analyst.

### Who is this for?

- **Travelers** — plan multimodal journeys across European cities with real-time departure awareness
- **Urban Explorers** — discover nearby transit options and understand local transit networks
- **Transit Analysts** — research operator networks, service patterns, and GTFS data
- **MaaS Developers** — integrate booking and trip planning into mobility applications


## Available Tools
- **get_arrivals**: Returns list of arriving services with line names and numbers, origins, scheduled and real-time arrival times (ETA), platform or bay information, delay indicators, and operator details. Essential for passenger pickup coordination, arrival monitoring, transit hub management, and real-time arrival boards. AI agents use this when users ask "when does the next train arrive at X", "show incoming services at this station", or need to track arriving services for passenger coordination.

Get upcoming arrivals at a specific transit stop
- **book_trip**: Supports booking train tickets, bus tickets, bike-sharing rentals, car-sharing reservations, and other mobility services available through the Lyko Book platform. Returns booking confirmation, payment details, ticket information, QR codes for validation, and cancellation policies. Availability and booking capabilities vary by operator and service type. Essential for Mobility-as-a-Service integration, ticket purchasing, service reservations, and end-to-end journey planning with booking. AI agents should use this when users ask "book this train ticket", "reserve a bike for this trip", or want to complete a mobility service reservation after planning a route.

Book a transit trip or mobility service through Lyko Book
- **get_departures**: Returns list of departing services with line names and numbers, destinations, scheduled and real-time departure times (ETD), platform or bay information, delay indicators, and operator details. Supports buses, trains, trams, subways, and ferries across European transit networks. Essential for passenger information displays, departure boards, travel apps, and real-time transit monitoring. AI agents should reference this when users ask "when is the next bus from stop X", "show departures from this station", or need to monitor upcoming services at a known transit stop.

Get next departures from a specific transit stop
- **get_line_info**: Returns line name, number, type (bus, train, tram, subway, ferry), operator, color code, route description, service hours, frequency, and accessibility information. Essential for line identification, transit network exploration, service information queries, and route planning context. AI agents should reference this when users ask "tell me about line M1", "what operator runs bus line 42", or need line metadata to understand transit service characteristics.

Get information about a specific transit line
- **get_line_routes**: Returns route variants (e.g., direction A and B), complete stop sequences with order, scheduled frequencies, first and last service times, and any service variations (express vs. local, peak vs. off-peak). Essential for complete line visualization, stop sequence analysis, transit mapping, and understanding service patterns. AI agents use this when users ask "show me all stops on line X", "what is the full route of bus 42", or need to understand complete service patterns for a transit line.

Get all routes and stops for a specific transit line
- **get_nearby_stops**: Returns nearby stops with distances from the coordinate, stop names, locations, served lines, operators, and stop types, sorted by proximity. Essential for location-based transit discovery, passenger navigation, "stops near me" features, and geographic transit analysis. AI agents use this when users ask "what stops are near my current location", "find transit stops within 500m of these coordinates", or need to discover accessible transit options from a specific point.

Find transit stops near a geographic location
- **get_network_status**: Returns active service disruptions, planned works, line closures, delay information, weather impacts, strike notifications, and alternative service recommendations. Essential for real-time service monitoring, disruption awareness, passenger communication, and travel planning during service changes. AI agents should reference this when users ask "are there any disruptions on SNCF trains", "is the Berlin U-Bahn running normally", or need to check service reliability before planning trips.

Get current network status and service alerts for a transit operator
- **get_operators**: Returns operator names, IDs, countries, coverage areas, transport modes operated (bus, train, tram, subway, ferry), contact information, and service status. Covers 300+ operators across Europe including SNCF (France), DB (Germany), NS (Netherlands), RENFE (Spain), Trenitalia (Italy), and many regional and local operators. Essential for operator research, transit network scoping, country-specific transit analysis, and understanding service coverage. AI agents should use this when users ask "what transit operators are available in France", "list all train operators in Germany", or need to identify operators for a specific country or region.

List public transit operators available in a country or region
- **plan_trip**: Supports multiple transport modes including buses, trains, subways, trams, ferries, bike-sharing, car-sharing, and walking combinations. Returns complete itinerary with departure and arrival times, duration, number of transfers, legs with mode details (line name, operator, vehicle type), intermediate stops, walking distances, fares if available, and real-time delay information. Essential for travel planning, multimodal journey optimization, passenger information systems, and Mobility-as-a-Service (MaaS) applications. AI agents should use this when users ask "how do I get from X to Y by public transport", "plan a trip from Paris Gare du Nord to Versailles", or need intermodal route options with timing and transfer details.

Plan an intermodal trip between two locations using public transit
- **search_stops**: Returns matching stops with stop IDs, names, locations (latitude, longitude), served lines, operators, and stop types. Essential for stop discovery, journey planning interfaces, transit stop identification, and building location-based transit features. AI agents should use this when users ask "find the bus stop near Champs-Elysees", "search for stops called X", or need to identify stop IDs for use in departure/arrival queries.

Search for transit stops by name or location
- **get_stop_info**: Returns stop name, location (latitude, longitude, address), served lines and routes, stop type (bus stop, train station, tram stop, subway station, ferry terminal), operator information, accessibility features (wheelchair access, elevators), and available amenities. Essential for stop identification, accessibility planning, transit network analysis, and passenger information. AI agents should use this when users ask "tell me about this stop", "what lines serve stop X", or need detailed stop metadata to contextualize transit queries.

Get detailed information about a specific transit stop
- **get_transit_feed**: Returns feed metadata, last update timestamp, included operators, coverage area, data freshness indicators, and download or access URLs. GTFS feeds contain static schedule data, route definitions, stop locations, fare information, and service calendars. Essential for transit data analysis, offline planning applications, academic research, and transit network visualization. AI agents use this when users need access to raw GTFS data, want to analyze transit schedules offline, or require complete network definitions for planning applications.

Access GTFS transit feed data for a specific operator or region


## Installation & Usage

To install and use the **Lyko** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lyko](https://vinkius.com/mcp/lyko)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
