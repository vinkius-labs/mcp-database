# AirLabs MCP Server

Access global aviation data via AirLabs — track real-time flights, search airports and airlines, check schedules, and analyze routes from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/airlabs)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

## Description
Connect your **AirLabs Data API** aviation platform to any AI agent and take full control of real-time flight tracking, airport intelligence, airline research, and schedule analysis through natural conversation.

### What you can do

- **Real-Time Flight Tracking** — Search active flights worldwide by airline, flight number, aircraft registration, or geographic area
- **Flight Schedules** — Access complete timetables for airlines and airport pairs with frequency and days of operation
- **Flight Information** — Get detailed status for specific flights including gates, terminals, and timing data
- **Airport Database** — Search 50,000+ airports worldwide by country, city, IATA/ICAO code, or name
- **Airline Database** — Research airlines globally with fleet sizes, hub airports, and operational status
- **Route Networks** — Analyze complete route portfolios for any airline with origin-destination pairs
- **Fleet Composition** — Examine airline fleets with aircraft types, registrations, ages, and operational status
- **Nearby Airports** — Find airports near any geographic coordinate with distance calculations
- **Airport Delays** — Check current delay statistics and on-time performance for any airport
- **Aircraft Lookup** — Research individual aircraft by hex code with registration and specification details
- **Airport Autocomplete** — Quick airport search with type-ahead suggestions for user-friendly identification
- **Airport Flight Boards** — Monitor all arrivals or departures at any airport with complete flight lists

### How it works

1. Subscribe to this server
2. Enter your AirLabs API key (from your account dashboard)
3. Start tracking global aviation from Claude, Cursor, or any MCP-compatible client

No more navigating flight tracking websites or manually parsing aviation data feeds. Your AI acts as a dedicated aviation data analyst and operations coordinator.

### Who is this for?

- **Aviation Enthusiasts** — track any flight worldwide, research aircraft, and explore airline fleets
- **Travel Planners** — check schedules, monitor flights, and assess airport delays for trip planning
- **Airline Analysts** — analyze competitor route networks, fleet composition, and operational performance
- **Airport Operators** — monitor flight activity, delay trends, and operational efficiency


## Available Tools
- **get_aircraft**: Returns aircraft registration number, ICAO type code, manufacturer and model, owner/operator, registration country, year built, engine type and count, and current operational status. The hex code is a unique identifier assigned to each aircraft transponder and can be found in flight tracking data. Essential for aviation enthusiasts, aircraft tracking, fleet verification, and detailed aircraft research. AI agents use this when users have an aircraft hex code from flight tracking data and need to look up the full aircraft registration and specifications.

Get information about a specific aircraft by hex code
- **get_airlines**: Supports filtering by country code, IATA code, ICAO code, airline name, or callsign. Returns airline details including IATA/ICAO codes, full name, country of registration, callsign, fleet size, founding year, hub airports, airline type (scheduled, cargo, charter), and operational status (active, inactive). Essential for airline industry research, competitor analysis, travel planning context, aviation market intelligence, and airline profile generation. AI agents should use this when users ask "show me all airlines in the US", "tell me about Lufthansa", "what airlines fly from Dubai", or need airline metadata to contextualize flight and fleet data.

Search and retrieve airline database information
- **get_airports**: Supports filtering by country code, city name, IATA code, ICAO code, airport name, or timezone. Returns airport details including IATA/ICAO codes, full name, location (city, state, country), geographic coordinates (latitude, longitude, elevation), timezone, airport type (large, medium, small), and operational status. Essential for airport identification, travel planning, geographic aviation research, multi-airport city analysis, and flight briefing preparation. AI agents should reference this when users ask "show me all airports in Germany", "find airports in Tokyo", "what is the ICAO code for Heathrow", or need airport metadata to contextualize flight queries.

Search and retrieve airport database information
- **autocomplete_airport**: Returns matching airports ranked by relevance with IATA/ICAO codes, full names, cities, countries, and airport types. Ideal for building airport search interfaces, type-ahead functionality, and airport identification when the user only knows part of the airport name or code. Essential for travel application development, airport search workflows, and user-friendly airport identification. AI agents should use this when users type partial airport names or codes and need quick suggestions, or when the exact airport code is unknown but a partial name is provided.

Search airports by name or code with autocomplete suggestions
- **get_airport_delays**: Returns average departure and arrival delays in minutes, delay trends compared to historical averages, on-time performance percentages, cancellation rates, and weather-related delay indicators. Essential for travel planning, delay prediction, passenger communication, airline operations coordination, and airport performance monitoring. AI agents should reference this when users ask "are there delays at JFK", "how is LAX performing today", or need to assess airport operational conditions that may affect flight schedules.

Get current delay statistics for a specific airport
- **get_airline_fleet**: Returns all aircraft in the airline fleet with registration numbers, aircraft types (manufacturer and model), ICAO aircraft type codes, age in years, delivery dates, engine types, and current operational status (active, stored, retired). Essential for fleet analysis, aviation industry research, competitor intelligence, aircraft utilization studies, and airline operational profiling. AI agents use this when users ask "show me the Delta fleet", "what aircraft does Emirates operate", or need to analyze fleet composition, average fleet age, and aircraft diversity for a specific airline.

Get the complete fleet composition of an airline
- **get_flight_info**: g., "UA123" for United 123). Returns complete flight details including airline information, aircraft type and registration, departure and arrival airports with terminals and gates, scheduled and estimated/actual times, current flight status, delay indicators, and baggage claim information. Critical for passenger travel updates, detailed flight status queries, airline operations coordination, and travel itinerary verification. AI agents should use this when users ask "tell me about flight UA123", "what is the status of BA178", or need detailed information for a specific flight number.

Get detailed information for a specific flight
- **get_flights_by_airport**: Returns comprehensive flight lists with airline, flight number, aircraft type, origin/destination airport, scheduled and estimated/actual times, terminal and gate information, baggage claim (for arrivals), and current flight status (en-route, landed, scheduled, delayed, cancelled, diverted). Supports type parameter to filter by "departure" or "arrival" flights. Essential for airport operations management, passenger pickup coordination, ground handling planning, flight activity monitoring, and arrival/departure board displays. AI agents should reference this when users ask "what flights are departing from JFK", "show me all arrivals at LHR", or need to monitor airport traffic for a specific airport.

Get all arriving or departing flights at a specific airport
- **get_flights**: Supports filtering by airline IATA code (e.g., "UA" for United), flight number, aircraft registration (hex code), altitude range, speed, or geographic bounding box (lat/lng coordinates). Returns flight identification (flight IATA/ICAO codes), airline details, aircraft hex code and registration, departure and arrival airports with IATA/ICAO codes, scheduled and estimated/actual times, current position (latitude, longitude), altitude in meters, ground speed in km/h, heading direction, vertical speed, squawk code, and flight status (en-route, landed, scheduled, cancelled). Essential for real-time flight tracking, passenger pickup coordination, aviation operations monitoring, and live flight dashboards. AI agents should use this when users ask "show me all United flights", "track flights in this area", or need to search flights by airline, registration, or geographic area.

Search for real-time active flights worldwide
- **get_nearby_airports**: Returns all airports (large international, regional, and general aviation) within the search radius with distances from the coordinate, IATA/ICAO codes, names, locations, and airport types. Essential for travel planning, alternate airport identification, geographic aviation research, emergency diversion planning, and multi-airport city analysis. AI agents should use this when users ask "what airports are near these coordinates", "find airports within 100km of this location", or need to identify the nearest airports to a specific point for travel or logistics purposes.

Find airports near a specific geographic location
- **get_airline_routes**: Returns route pairs (origin-destination airports), frequency of service, days of operation, aircraft types deployed on each route, and whether the route is seasonal or year-round. Essential for route network analysis, airline competitive intelligence, aviation market research, travel itinerary planning, and airline hub/spoke structure analysis. AI agents should reference this when users ask "show me all United routes", "what routes does Ryanair operate", or need to understand an airline route network for competitive analysis or travel planning.

Get all routes operated by a specific airline
- **get_schedules**: Returns scheduled flights with airline, flight number, aircraft type, departure and arrival airports, scheduled times, frequency of service, days of operation, and aircraft registration if assigned. Supports filtering by airline IATA code, departure airport IATA, arrival airport IATA, date range, and flight number. Essential for travel planning, route analysis, schedule reliability studies, airline timetable research, and flight itinerary preparation. AI agents should reference this when users ask "what is the schedule from JFK to LAX", "show me all Delta flights from ATL", or need to analyze flight schedules between airports.

Get flight schedules and timetables for airlines and airports


## Installation & Usage

To install and use the **AirLabs** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airlabs](https://vinkius.com/mcp/airlabs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
