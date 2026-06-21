# FlightAware MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flightaware)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Track global flight status via FlightAware AeroAPI — search flights, monitor airport arrivals and departures, check weather, and access historical flight data from any AI agent.

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


## Available Tools (12)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FlightAware** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all active United Airlines flights from Newark (KEWR) to San Francisco (KSFO)."

**🤖 AI Agent:**
> Searching FlightAware... I found 5 active United flights on the KEWR-KSFO route today: UA123 (Boeing 737-900, departed KEWR 08:15 EST, en-route at FL370, ETA KSFO 11:42 PST), UA456 (Boeing 757-200, departed 10:30 EST, en-route at FL350, ETA 14:05 PST), UA789 (Airbus A320, departed 13:45 EST, currently climbing through FL280, ETA 17:18 PST), UA234 (Boeing 737-MAX 9, scheduled departure 16:20 EST), and UA567 (Boeing 787-9, scheduled 19:00 EST). Would you like detailed gate and terminal information for any of these flights?

---

**👤 You:**
> "What is the current weather at Chicago O'Hare (KORD) and are flights being delayed due to conditions?"

**🤖 AI Agent:**
> Checking KORD weather and flight status... Current METAR observation at Chicago O'Hare: Wind 270 degrees at 18 knots gusting to 28, visibility 6 statute miles in light snow, broken clouds at 2500 feet, overcast at 4000 feet, temperature minus 4 Celsius, dewpoint minus 8, altimeter 29.87 inches Hg. Reviewing arrivals and departures: I'm seeing average delays of 25-40 minutes for inbound flights due to low ceiling and gusty crosswind conditions on runways 10L/28R. Several flights have been diverted to alternate airports (MDW, RFD). Outbound flights are experiencing similar delays with ground stops imposed periodically. Would you like me to monitor specific flights for you?

---

**👤 You:**
> "Show me the complete flight history and track points for British Airways flight BAW117 from London to New York yesterday."

**🤖 AI Agent:**
> Retrieving historical flight data for BAW117... Flight BAW117 (Boeing 777-300ER, registration G-STBF) departed London Heathrow (EGLL) at 2025-04-08 10:12 UTC (scheduled 10:05 UTC, 7 minutes early) from Terminal 5 Gate A12. The flight tracked westbound across the North Atlantic via the NATS track system, filing route: KONAN L607 RESNO 52N020W 52N030W 51N040W 50N050W 49N060W J547 CAM J753 MERIT. Cruising altitude FL380 with average ground speed 485 knots. Arrived New York JFK (KJFK) at 2025-04-08 13:28 UTC (scheduled 13:45 UTC, 17 minutes early) at Terminal 7 Gate 1. Total flight time: 7 hours 16 minutes. Complete track log contains 432 position points. Would you like me to generate a route map or analyze performance metrics for this crossing?


## ❓ FAQ

**Q: Can my AI track a specific flight in real-time and tell me exactly where it is, its altitude, and estimated arrival time?**
Yes! Use the `search_flights` tool with the flight number (e.g., "UAL123") or tail number to find active flights. Your AI agent will respond with current position coordinates, ground speed, altitude, estimated time of arrival (ETA), departure and arrival airports with gates, and whether the flight is en-route, landed, or experiencing delays. For even more detail on a specific flight, use `get_flight_status` with the FlightAware ID to get complete operational metadata.

**Q: How do I check all arriving and departing flights at a specific airport along with current weather conditions?**
Simply ask the agent to run the `get_airport_arrivals` and `get_airport_departures` actions with the airport ICAO code (e.g., "KJFK" for New York JFK, "KLAX" for Los Angeles). Then request `get_airport_weather` for the same airport to see current METAR observations including wind, visibility, ceiling, temperature, and any weather phenomena affecting operations. The AI will compile a complete picture of airport activity and meteorological conditions.

**Q: Can I access historical flight data to analyze on-time performance and typical routes flown between two cities?**
Absolutely! Use the `get_historical_flights` tool with a FlightAware canonical flight ID to retrieve complete flight history dating back to January 1, 2011. You'll get actual departure and arrival times, delay indicators, the route flown, and all track points with timestamps. To understand common routing patterns between airports, use `get_airport_routes` with origin and destination ICAO codes to see frequently filed routes. This is perfect for schedule reliability studies, aviation trend analysis, and operational benchmarking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flightaware](https://vinkius.com/mcp/flightaware)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FlightAware** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flightaware` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FlightAware** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flightaware": {
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
