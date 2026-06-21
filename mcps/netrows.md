# Netrows MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netrows)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track global flights via Netrows Aviation API — search flights, monitor aircraft, check airport data, and access airline schedules from any AI agent.

## Description
Connect your **Netrows Aviation API** flight tracking platform to any AI agent and take full control of real-time flight monitoring, aircraft intelligence, airport operations, and airline schedule analysis through natural conversation.

### What you can do

- **Flight Search** — Find active and recent flights by flight number, callsign, or origin-destination airport pair
- **Flight Details** — Get comprehensive flight information including airports, times, aircraft, and status
- **Real-Time Tracking** — Monitor live flight positions with coordinates, altitude, speed, and heading
- **Aircraft Registry** — Look up aircraft specifications, ownership, registration, and fleet details
- **Fleet Analysis** — Search all aircraft operated by specific airlines or aviation companies
- **Airport Intelligence** — Query airport static data, codes, locations, and timezone information
- **Airport Activity** — Monitor all arriving and departing flights at any airport worldwide
- **Airport Search** — Find all airports serving a specific city or metropolitan area
- **Flight Schedules** — Access complete flight schedules between any two airports
- **Airline Monitoring** — Track all active flights by airline with real-time operational data
- **Airline Profiles** — Get airline company information including fleet size, hubs, and destinations
- **Account Usage** — Monitor your API credit consumption and remaining quota

### How it works

1. Subscribe to this server
2. Enter your Netrows API key (from the Developer Portal)
3. Start tracking global aviation from Claude, Cursor, or any MCP-compatible client

No more navigating flight tracking websites or manually parsing aviation data feeds. Your AI acts as a dedicated aviation analyst and flight operations coordinator.

### Who is this for?

- **Aviation Enthusiasts** — track any flight worldwide, research aircraft details, and explore airline fleets
- **Travel Planners** — monitor arriving and departing flights for passenger pickup and delay awareness
- **Airport Operators** — observe real-time airport activity and traffic patterns
- **Airline Analysts** — track competitor operations, analyze route networks, and monitor fleet utilization


## Available Tools
- **get_account_usage**: The Netrows API operates on a credit-based system where each API call consumes 1 credit. Essential for monitoring API consumption, budget management, rate limit awareness, and planning integration usage patterns. AI agents should query this when users ask "how many credits do I have left", "what is my API usage this month", or need to monitor their API consumption before running large batch queries.

Check your API account usage and remaining credits
- **get_aircraft_info**: g., "N12345" for US-registered, "G-EUUU" for UK). Returns aircraft type (manufacturer and model), registration country, owner/operator information, registration status, year built, engine type (jet, turboprop, piston), number of engines, aircraft age, and category (airline, business jet, private, cargo). Critical for aviation enthusiasts, fleet tracking, aircraft utilization analysis, and private aviation monitoring. AI agents should reference this when users ask "tell me about aircraft N12345", "who owns this tail number", or need aircraft specifications to contextualize flight data.

Get registration details and specifications for a specific aircraft
- **get_airline_flights**: g., "UA" for United, "DL" for Delta, "BA" for British Airways). Returns flight numbers, aircraft registrations and types, origin-destination pairs, scheduled and actual times, and current status for all flights in the airline fleet. Essential for airline operations monitoring, fleet utilization analysis, competitor intelligence, and passenger rebooking during disruptions. AI agents use this when users ask "show me all United flights right now", "what is Delta flying", or need to track an entire airline operational picture in real-time.

List all active flights operated by a specific airline
- **get_airport_flights**: Returns a comprehensive list of inbound and outbound flights with airline/operator, flight number, aircraft type, origin/destination airports, scheduled and actual times, and current flight status (en-route, landed, scheduled, delayed, cancelled, diverted). Essential for airport operations management, passenger pickup coordination, ground handling planning, and flight activity monitoring. AI agents should reference this when users ask "what flights are at X airport", "show me all activity at Y", or need to monitor airport traffic patterns.

List all arriving and departing flights at a specific airport
- **get_airline_info**: Returns airline name, IATA/ICAO codes, callsign, country of registration, fleet size, destination count, hub airports, and operational status. Essential for airline industry research, competitor analysis, travel planning context, and aviation market intelligence. AI agents should reference this when users ask "tell me about United Airlines", "what is the ICAO code for Delta", or need airline metadata to contextualize flight and fleet data.

Get information and details for a specific airline
- **get_airport_info**: g., "JFK" or "KJFK" for New York JFK, "LAX" or "KLAX" for Los Angeles International). Returns airport name, location (city, state, country), IATA/ICAO/FAA codes, geographic coordinates (latitude, longitude, elevation), timezone, and operational status. Essential for airport identification, travel planning, flight briefing preparation, and geographic reference. AI agents should use this when users ask "tell me about airport X", "what is the ICAO code for Y", or need airport metadata to contextualize flight queries.

Get static information and details for a specific airport
- **get_flight_details**: Returns departure and arrival airports with full metadata (IATA/ICAO codes, terminal, gate), scheduled and actual times for departure and arrival, aircraft registration and type, airline/operator details, current flight status, and tracking coordinates if airborne. Critical for passenger travel updates, airline operations coordination, and flight tracking dashboards. AI agents should reference this when users request detailed status for a known flight, including gate assignments, timing comparisons, and aircraft information.

Get complete details for a specific flight
- **get_flight_schedule**: Returns all scheduled flights with airline/operator, flight numbers, aircraft types, departure and arrival times, frequency of service, and days of operation. Essential for route planning, travel itinerary preparation, schedule analysis, and aviation market research. AI agents should reference this when users ask "what flights fly from JFK to LAX", "show me the schedule between ORD and DFW", or need to plan travel between specific airport pairs with comprehensive scheduling options.

Get scheduled flights between two airports
- **search_aircraft**: Returns all registered aircraft in the operator fleet with registration numbers, aircraft types (manufacturer and model), ages, and current operational status. Essential for fleet analysis, aviation industry research, competitor intelligence, and operator profile generation. AI agents use this when users ask "show me all United Airlines aircraft", "what planes does Delta operate", or need to analyze fleet composition for a specific aviation operator.

Search for all aircraft operated by a specific airline or company
- **search_airports**: Returns all airports (major international, regional, and general aviation) associated with the queried city including IATA/ICAO codes, full names, locations, distances from city center, and airport types. Essential for travel planning, multi-airport city analysis, alternate airport identification, and geographic aviation research. AI agents use this when users ask "what airports serve Chicago", "find airports in London", or need to identify all airports in a metropolitan area for comprehensive flight searches.

Search for airports by city name or location
- **search_flights**: The query can be a flight number (e.g., "UAL123"), callsign, or origin-destination airport pair. Returns complete flight identification, airline/operator, aircraft type, departure and arrival airports with IATA/ICAO codes, scheduled and actual times, current position coordinates (latitude, longitude), altitude in feet, ground speed in knots, heading, and flight status (en-route, landed, diverted, cancelled). Essential for real-time flight tracking, passenger pickup coordination, logistics planning, and aviation operations monitoring. AI agents should use this when users ask "where is flight X", "what flights are flying from A to B", or need to track specific flights by number or route.

Search for active and recent flights by flight number, callsign, or route
- **track_flight**: Returns timestamped position data that can be used to visualize flight progress on maps, estimate arrival times, and monitor flight trajectory. Essential for live flight tracking applications, passenger monitoring, operations dashboards, and aviation enthusiast displays. AI agents use this when users ask "track this flight live", "where is this aircraft right now", or need continuous position updates for an airborne flight.

Track real-time position and status of a specific flight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Netrows** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all active United Airlines flights from Newark to San Francisco."

**🤖 AI Agent:**
> Searching Netrows Aviation API... I found 5 active United flights on the EWR-SFO route today: UA123 (Boeing 737-900, departed EWR 08:15 EST, en-route at FL370, ETA SFO 11:42 PST), UA456 (Boeing 757-200, departed 10:30 EST, en-route at FL350, ETA 14:05 PST), UA789 (Airbus A320, departed 13:45 EST, currently climbing through FL280, ETA 17:18 PST), UA234 (Boeing 737-MAX 9, scheduled departure 16:20 EST), and UA567 (Boeing 787-9, scheduled 19:00 EST). Would you like detailed tracking data for any of these flights?

---

**👤 You:**
> "Show me all airports that serve the city of London and their current flight activity."

**🤖 AI Agent:**
> Searching London airports... I found 6 airports serving the London metropolitan area: London Heathrow (LHR/EGLL) — 412 flights today (268 arrivals, 144 departures), London Gatwick (LGW/EGKK) — 287 flights (178 arrivals, 109 departures), London Stansted (STN/EGSS) — 195 flights (121 arrivals, 74 departures), London Luton (LTN/EGGW) — 143 flights (89 arrivals, 54 departures), London City (LCY/EGLC) — 98 flights (61 arrivals, 37 departures), and London Southend (SEN/EGMC) — 34 flights (21 arrivals, 13 departures). Total: 1,169 flights across all London airports today. Would you like detailed flight lists for any specific airport?

---

**👤 You:**
> "Tell me about aircraft N12345 — who owns it, what type is it, and what flights has it been operating?"

**🤖 AI Agent:**
> Looking up aircraft N12345... This is a Boeing 737-800 (registration N12345) registered in the United States, operated by United Airlines. Built in 2018 (6 years old), equipped with 2 CFM56-7B jet engines. Aircraft category: Commercial Airline. Current status: Active. Recent flight activity shows this aircraft has been primarily operating United domestic routes including EWR-LAX, SFO-IAH, and ORD-DEN. Would you like me to track its current flight or show its complete recent flight history?


## ❓ FAQ

**Q: Can my AI track a specific flight in real-time and show me its current position, altitude, and speed?**
Yes! Use the `search_flights` tool with the flight number (e.g., "UAL123") to find the active flight, then use `track_flight` with the flight ID to get real-time position coordinates (latitude, longitude), altitude in feet, ground speed in knots, heading direction, and vertical speed. Your AI agent will respond with the exact location of the aircraft and its current flight parameters. Perfect for passenger pickup coordination and live flight monitoring.

**Q: How do I find all flights departing from or arriving at a specific airport?**
Simply ask the agent to run the `get_airport_flights` action with the airport IATA or ICAO code (e.g., "JFK" or "KJFK" for New York JFK). It will return all arriving and departing flights with airline, flight number, aircraft type, origin/destination, scheduled and actual times, and current status. You can also use `search_airports` first to find the correct airport code if you only know the city name.

**Q: Can I look up information about a specific aircraft by its tail number or registration?**
Absolutely! Use the `get_aircraft_info` tool with the aircraft registration/tail number (e.g., "N12345" for US, "G-EUUU" for UK, "D-AIMA" for Germany). Your AI will return the aircraft manufacturer and model, registration country, owner/operator, year built, engine type, number of engines, aircraft age, and category (airline, business jet, private, cargo). You can also use `search_aircraft` with an operator name to see their entire fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netrows](https://vinkius.com/mcp/netrows)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Netrows** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `netrows` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Netrows** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "netrows": {
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
