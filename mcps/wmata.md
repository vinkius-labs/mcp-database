# WMATA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wmata)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access Washington DC Metro data via WMATA — track Metrorail and Metrobus in real-time, check incidents, and plan station visits from any AI agent.

## Description
Connect your **WMATA API** Washington DC public transit data platform to any AI agent and take full control of real-time Metrorail and Metrobus tracking, incident monitoring, and station information through natural conversation.

### What you can do

- **Next Rail Predictions** — Get real-time next train predictions system-wide or at specific Metrorail stations
- **Station Discovery** — List all Metrorail stations with codes, addresses, coordinates, and line affiliations
- **Station Predictions** — Get detailed next train arrivals at any specific Metrorail station
- **Metrobus Tracking** — Track real-time GPS positions of all Metrobus vehicles or filter by route
- **Bus Route Details** — Get complete route information including stop sequences for any Metrobus route
- **Rail Incidents** — Monitor active service disruptions affecting Metrorail lines and stations
- **Bus Incidents** — Check current incidents and detours affecting Metrobus service
- **Elevator Outages** — Track elevator and escalator outages for accessibility planning
- **Station Entrances** — Get street-level entrance information for any Metrorail station
- **Parking Lots** — Find station parking availability, fees, and amenities for park-and-ride planning
- **Bus Routes** — Browse all Metrobus routes operating across DC, Maryland, and Virginia
- **Bus Predictions** — Get next bus arrival predictions at stations and stops

### How it works

1. Subscribe to this server
2. Enter your WMATA API key (free from the Developer Portal)
3. Start tracking DC Metro transit from Claude, Cursor, or any MCP-compatible client

No more navigating the Metro website or manually checking train times. Your AI acts as a dedicated DC transit analyst and trip planning assistant.

### Who is this for?

- **DC Commuters** — track trains and buses, check incidents, and plan park-and-ride trips
- **Tourists** — navigate the Metrorail system with station discovery and entrance guidance
- **Accessibility Planners** — verify elevator status and accessible entrances before traveling
- **Transit Apps** — integrate real-time WMATA data into mobility and journey planning applications


## Available Tools
- **get_bus_incidents**: Returns incident descriptions, affected route IDs, detour information, bus stop closures, incident types (accident, road closure, construction, mechanical), start timestamps, and alternative service recommendations. Essential for bus service disruption awareness, alternative route planning, and passenger communication. AI agents should use this when users ask "are there any bus delays", "is route 30N running normally", or need to check Metrobus service reliability.

Get current incidents affecting Metrobus service
- **get_bus_positions**: Returns bus vehicle IDs, route IDs, latitude/longitude coordinates, trip IDs, destination names, deviation from schedule in seconds, and direction. Can query all buses system-wide or filter by specific route ID. Essential for real-time bus tracking, passenger wait time estimation, and bus arrival prediction. AI agents should reference this when users ask "where is the X2 bus", "show all buses on route 30N", or need to track Metrobus vehicles in real-time. Route IDs are typically 2-5 character identifiers (e.g., "30N", "X2", "L2"). Use getBusRoutes first to find route IDs if unknown.

Get real-time positions of Metrobus vehicles, optionally filtered by route
- **get_bus_route_details**: Returns all stops served by the route in order, trip headsigns, and route path information. Essential for route planning, understanding bus service coverage, stop discovery, and passenger journey preparation. AI agents should use this when users ask "what stops does the 30N bus serve", "show me the route details for X2", or need complete route structure including stop sequences for trip planning.

Get detailed information about a specific Metrobus route
- **get_bus_routes**: Returns route IDs, route names, descriptions, and route types. Covers all WMATA-operated bus routes including limited-stop, local, and express services across DC, Maryland, and Virginia. Essential for route discovery, service area analysis, transit network understanding, and identifying route IDs for use in bus position and route detail queries. AI agents should reference this when users ask "list all bus routes", "what bus routes serve DC", or need to identify route IDs for subsequent Metrobus queries.

List all Metrobus routes in the WMATA system
- **get_circuit_predictions**: Returns bus route IDs, destination names, predicted arrival times in minutes, trip IDs, and vehicle IDs. Supports filtering by station code for station-specific predictions or system-wide queries. Essential for bus trip planning, real-time bus arrival awareness, and connection coordination between Metrorail and Metrobus. AI agents should use this when users ask "when is the next bus at Union Station", "show bus predictions for Foggy Bottom", or need real-time bus arrival predictions at a specific station or stop.

Get next bus arrival predictions for Metrobus Circuit routes
- **get_elevator_incidents**: Returns affected station codes and names, elevator/escalator identifiers, outage descriptions, estimated repair times, outage start timestamps, and accessibility impact information. Essential for accessibility planning, wheelchair route verification, senior and disability passenger support, and station accessibility awareness. AI agents should use this when users ask "are there any elevator outages at Gallery Place", "is the elevator working at Union Station", or need to verify station accessibility before planning journeys for passengers with mobility needs.

Get current elevator and escalator outages at Metrorail stations
- **get_next_rail**: Returns train destination names, lines (Red, Orange, Silver, Blue, Yellow, Green), predicted arrival times in minutes, car counts, group numbers, and train direction. Can query all trains system-wide or filter by specific station code. Essential for commuter trip planning, real-time arrival awareness, and station crowd management. AI agents should use this when users ask "when is the next train", "show upcoming trains at Gallery Place", or need real-time Metrorail arrival predictions. Station codes are 3-letter identifiers (e.g., "A01" for Metro Center, "B36" for Gallery Place). Use getRailStations first to find station codes if unknown.

Get next train predictions across the entire Metrorail system or at a specific station
- **get_parking_lots**: Can query all parking lots system-wide or filter by specific station code. Essential for park-and-ride trip planning, commuter parking availability, station selection for driving passengers, and transportation mode choice analysis. AI agents should use this when users ask "which stations have parking", "how many spaces are at Shady Grove", or need to plan park-and-ride journeys from suburban areas into DC.

Get Metrorail station parking lot information
- **get_rail_incidents**: Returns incident descriptions, affected station codes, line impacts, incident types (delay, power problem, medical, police activity, track maintenance), severity indicators, start timestamps, and estimated resolution times. Essential for service disruption awareness, alternative route planning, passenger communication, and understanding system reliability. AI agents should reference this when users ask "are there any delays on the Red Line", "is Metro running normally", or need to check service reliability before planning Metrorail journeys.

Get current incidents affecting Metrorail service
- **get_rail_stations**: Can filter by line code (RD=Red, OR=Orange, SV=Silver, BL=Blue, YL=Yellow, GR=Green) to show only stations on that line. Essential for station discovery, route planning, understanding line structure, and mapping the Metrorail network. AI agents should reference this when users ask "list all stations on the Red Line", "what is the station code for Foggy Bottom", or need to understand station sequences and line geography. Station codes are required for subsequent queries like next trains, predictions, entrances, and parking.

List all Metrorail stations, optionally filtered by line
- **get_station_entrances**: Returns entrance names, street addresses, latitude/longitude coordinates, entrance descriptions, and whether the entrance has escalator or elevator access. Essential for station navigation, first-time visitor guidance, street-level wayfinding, accessible entrance identification, and trip end planning. AI agents should reference this when users ask "where are the entrances to Metro Center", "find the closest entrance to Gallery Place", or need street-level navigation guidance for reaching a Metrorail station.

Get entrance information for a specific Metrorail station
- **get_station_prediction**: Returns trains with destination names, line colors, predicted arrival times, car counts, and train direction. More targeted than system-wide next rail queries. Essential for passenger waiting at a specific station, connection planning, and real-time arrival boards. AI agents should use this when users ask "when is the next train at Silver Spring", "show trains coming to Shady Grove", or need station-specific arrival predictions. Requires station code from getRailStations results.

Get next train predictions at a specific Metrorail station


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WMATA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the next trains arriving at Gallery Place station."

**🤖 AI Agent:**
> Fetching predictions for Gallery Place (B36)... Next trains: Red Line to Glenmont — 2 minutes, 8 cars; Red Line to Shady Grove — 4 minutes, 6 cars; Yellow Line to Greenbelt — 6 minutes, 6 cars; Green Line to Branch Ave — 8 minutes, 6 cars; Yellow Line to Huntington — 10 minutes, 4 cars. All services operating on schedule with no delays reported.

---

**👤 You:**
> "Are there any incidents affecting the Red Line right now?"

**🤖 AI Agent:**
> Checking Metrorail incidents... Currently 1 active incident: Single-tracking between Twinbrook and Rockville due to track maintenance. Expect 10-15 minute delays in both directions. Estimated resolution: 2:30 PM. No other incidents reported on the Red Line. All other lines are operating normally. Would you like me to check elevator status at any Red Line stations?

---

**👤 You:**
> "Where is the closest entrance to Metro Center station from 12th Street?"

**🤖 AI Agent:**
> Fetching Metro Center (A01) entrances... Found 7 entrances. Closest to 12th Street: Entrance at 12th & G Streets NW — coordinates 38.8983, -77.0283, has escalator access. Also nearby: Entrance at 1155 Connecticut Ave NW — coordinates 38.9056, -77.0421, has elevator and escalator (accessible). Full list includes entrances on F Street, G Street, and Connecticut Avenue. Would you like walking directions from your current location to the closest entrance?


## ❓ FAQ

**Q: Can my AI check when the next Metrorail train is arriving at my station?**
Yes! Use the `get_station_prediction` tool with the station code (e.g., "A01" for Metro Center, "B36" for Gallery Place). Your AI will return all upcoming trains with destination names, line colors (Red, Orange, Silver, Blue, Yellow, Green), predicted arrival times in minutes, and car counts. If you do not know the station code, first use `get_rail_stations` to find it by name. For a system-wide view of all upcoming trains, use `get_next_rail` without a station code.

**Q: How do I check if there are any delays or incidents affecting my Metrorail line?**
Use the `get_rail_incidents` tool to check all active service disruptions across the Metrorail system. This returns incident descriptions, affected stations and lines, incident types (delays, power problems, medical emergencies, track maintenance), and start times. You can also check `get_elevator_incidents` for elevator and escalator outages that may affect accessibility at your station. For Metrobus service issues, use `get_bus_incidents`.

**Q: Can I track Metrobus vehicles in real-time to see when my bus will arrive?**
Yes! Use `get_bus_positions` to see real-time GPS locations of all Metrobus vehicles, or filter by route ID (e.g., "30N", "X2") to track buses on a specific route. Returns vehicle IDs, route IDs, latitude/longitude, destinations, and schedule deviation in seconds. For detailed route information including stop sequences, use `get_bus_route_details` with the route ID. Use `get_bus_routes` first to find route IDs if unknown.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wmata](https://vinkius.com/mcp/wmata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WMATA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wmata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WMATA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wmata": {
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
