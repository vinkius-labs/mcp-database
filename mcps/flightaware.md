# FlightAware MCP Server

Track global flight status via FlightAware AeroAPI — search flights, monitor airport arrivals and departures, check weather, and access historical flight data from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flightaware)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

## Description
Connect your **FlightAware AeroAPI** aviation data platform to any AI agent and take full control of global flight tracking, airport operations monitoring, and historical flight analysis through natural conversation.

### What you can do

- **Flight Search** — Find active and recent flights by flight number, tail number, or origin-destination pair
- **Flight Status** — Get complete status details including gates, runways, scheduled vs. actual times, and delay indicators
- **Route Tracking** — Access filed flight plans with all waypoints, airways, and altitude restrictions
- **Flight Maps** — Retrieve static map images showing complete flight tracks from departure to arrival
- **Airport Intelligence** — Query airport static data, arrivals, departures, and real-time weather observations
- **Airline Operations** — Monitor entire airline fleets with all active flights by operator/airline code
- **Aircraft Registry** — Look up aircraft specifications, ownership, registration status, and equipment type
- **Historical Analysis** — Access flight history dating back to 2011 with complete track points and performance data
- **Route Planning** — Discover commonly filed routes between any two airports for flight planning and research
- **Weather Impact** — Check METAR/TAF weather data to assess meteorological impact on flight operations

### How it works

1. Subscribe to this server
2. Enter your FlightAware AeroAPI API key (from the Developer Portal)
3. Start tracking global aviation from Claude, Cursor, or any MCP-compatible client

No more navigating flight tracking websites or manually parsing aviation data feeds. Your AI acts as a dedicated aviation analyst and operations coordinator.

### Who is this for?

- **Aviation Enthusiasts** — track any flight worldwide, look up aircraft details, and explore historical flight patterns
- **Travel Planners** — monitor arriving and departing flights for passenger pickup, connection tracking, and delay awareness
- **Airline Operations** — observe competitor fleet movements, analyze route networks, and assess operational disruptions
- **Flight Dispatchers** — verify filed routes, check weather at destination airports, and review historical performance data


## Available Tools
- **get_aircraft_info**: g., "N12345" for US-registered, "G-EUUU" for UK). Returns aircraft type (manufacturer and model), registration country, owner/operator information, registration status, year built, engine type (jet, turboprop, piston), number of engines, and category (airline, business jet, private, cargo, military). Critical for aviation enthusiasts, fleet tracking, aircraft utilization analysis, and private aviation monitoring. AI agents should reference this when users ask "tell me about aircraft N12345", "who owns this tail number", or need aircraft specifications to contextualize flight data.

Get registration details and specifications for a specific aircraft
- **get_airport_arrivals**: Returns a list of inbound flights with airline/operator, flight number, aircraft type, origin airport, scheduled and estimated/actual arrival times, arrival runway and gate, and current flight status (en-route, landed, delayed, cancelled, diverted). Essential for airport operations management, passenger pickup coordination, ground handling planning, and arrival delay monitoring. AI agents should reference this when users ask "what flights are arriving at X", "show me arrivals at Y airport", or need to track inbound flights for a specific destination.

List arriving flights at a specific airport
- **get_airport_departures**: Returns a list of outbound flights with airline/operator, flight number, aircraft type, destination airport, scheduled and estimated/actual departure times, departure runway and gate, and current flight status (scheduled, boarding, departed, delayed, cancelled, diverted). Critical for airport operations coordination, passenger departure monitoring, gate management, and departure delay tracking. AI agents use this when users ask "what flights are leaving from X", "show me departures at Y airport", or need to track outbound flights from a specific origin.

List departing flights from a specific airport
- **search_flights**: The query can be a flight number (e.g., "UAL123"), aircraft tail number/registration (e.g., "N12345"), or origin-destination pair (e.g., "KJFK-KLAX"). Returns complete flight identification, airline/operator, aircraft type, departure and arrival airports, scheduled and actual times, current position (if airborne), altitude, ground speed, and flight status (en-route, landed, diverted, cancelled). Essential for real-time flight tracking, passenger pick-up coordination, logistics planning, and aviation operations monitoring. AI agents should use this when users ask "where is flight X", "what flights are flying from A to B", or "show me all flights by tail number N".

Search for active and recent flights by flight number, tail number, or route
- **get_airport_info**: g., "KJFK" for New York JFK, "KLAX" for Los Angeles International). Returns airport name, location (city, state, country), ICAO/IATA/FAA/LID codes, geographic coordinates (latitude, longitude, elevation), timezone, runway information, and canonical FlightAware ID. Essential for airport identification, travel planning, flight briefing preparation, and geographic reference. AI agents should use this when users ask "tell me about airport X", "what is the ICAO code for Y", or need airport metadata to contextualize flight queries.

Get static information and details for a specific airport
- **get_airport_routes**: Returns route strings, frequency of use, typical altitudes, and associated flight examples. Essential for flight planning, route optimization analysis, aviation research, and pilot briefing preparation. AI agents should reference this when users ask "what routes are flown between X and Y", "show me common paths from JFK to LAX", or need to understand routing options between airport pairs for planning or analysis purposes.

Get routes between two specific airports
- **get_airport_weather**: Returns METAR (avi routine weather report) data including wind speed and direction, visibility, cloud layers, temperature, dewpoint, altimeter setting, present weather phenomena (rain, snow, fog, thunderstorms), and automated weather remarks. Also provides TAF (terminal aerodrome forecast) for upcoming weather conditions. Essential for flight planning, aviation safety assessment, delay prediction due to weather, and pilot briefing preparation. AI agents should query this when users ask "what is the weather at X airport", "is weather affecting flights at Y", or need to assess meteorological impact on flight operations.

Get current weather observations and forecast for a specific airport
- **get_flight_map**: The map shows the filed route, actual track points, departure and arrival airports, and current aircraft position (if airborne). Useful for visual flight presentation, passenger communication, operations dashboards, and flight tracking displays. AI agents should reference this when users request to "show me the flight path" or "where is this flight on a map". Returns image URL that can be embedded in responses or displayed directly.

Get a static map image showing the flight track
- **get_flight_route**: Returns the route as a structured list of fixes, navaids, and airway segments from departure to arrival airport. Essential for flight following, aviation enthusiast tracking, pilot briefing preparation, and route analysis. AI agents use this to visualize flight paths, compare filed routes against actual tracks, analyze common routing patterns between airport pairs, and provide pilots with route reference data.

Get the filed flight plan route for a specific flight
- **get_flight_status**: Returns departure and arrival airports with terminals and gates, scheduled/estimated/actual times for pushback, takeoff, landing, and arrival, current flight status (en-route, landed, diverted, cancelled, in-hold), delay indicators, aircraft registration and type, route description, and diversion airports if applicable. Critical for passenger travel updates, airline operations coordination, and flight tracking dashboards. AI agents should reference this when users request detailed status for a known flight ID, including gate assignments, delay reasons, and actual vs. scheduled time comparisons.

Get complete status details for a specific flight
- **get_historical_flights**: Access continuous flight history data dating back to January 1, 2011, including actual departure and arrival times, route flown, all track points (latitude, longitude, altitude, ground speed, timestamp), arrival status, and delay indicators. Essential for post-flight analysis, operational trend identification, schedule reliability assessment, on-time performance tracking, and aviation safety investigations. AI agents use this when users ask "show me the history of flight X", "how has this route performed over time", or need to analyze historical flight patterns for reliability studies.

Get historical flight data and track for a specific flight
- **get_operator_flights**: g., "UAL" for United Airlines, "DAL" for Delta, "BAW" for British Airways). Returns flight numbers, aircraft types, origin-destination pairs, scheduled and actual times, and current status for all flights in the operator fleet. Essential for airline operations monitoring, fleet utilization analysis, competitor intelligence, and passenger rebooking during disruptions. AI agents use this when users ask "show me all United flights", "what is Delta flying right now", or need to track an entire airline operational picture.

List all flights operated by a specific airline or operator


## Installation & Usage

To install and use the **FlightAware** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flightaware](https://vinkius.com/mcp/flightaware)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
