# Navitia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/navitia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/navitia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/navitia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation-logistics](../categories/transportation-logistics.md)

Access European public transit via Navitia — plan multimodal journeys, check schedules, track disruptions, and explore transit networks from any AI agent.

## Description
Connect your **Navitia** multimodal transit API to any AI agent and take full control of European public transportation planning, real-time service monitoring, and accessibility analysis through natural conversation.

### What you can do

- **Multimodal Journey Planning** — Plan door-to-door trips combining metro, bus, tram, RER, regional rail, walking, cycling, bike-sharing, and car
- **Place Search** — Find transit stops, stations, addresses, and POIs with autocomplete search across French and European networks
- **Real-Time Departures** — Check upcoming departures at any transit stop with ETAs, platforms, and delay indicators
- **Arrival Tracking** — Monitor incoming services for passenger pickup and connection coordination
- **Stop Schedules** — Access complete timetables for any transit stop with weekday/weekend/holiday patterns
- **Nearby Discovery** — Find all transit stops near any geographic coordinate with distance calculations
- **Service Disruptions** — Check active alerts, strikes, maintenance works, and operational notices across networks
- **Line Exploration** — Browse all transit lines by mode type (metro, bus, tram, rail) with operator affiliations
- **Network Analysis** — Research transit operators including RATP, SNCF, TCL, RTM, and regional authorities
- **Isochrone Mapping** — Generate accessibility maps showing reachable areas within time limits from any point
- **Coverage Discovery** — List all available coverage regions with data validity periods and contributor information

### How it works

1. Subscribe to this server
2. Enter your Navitia API key (from the developer portal or your Public Transport Authority)
3. Start planning European transit journeys from Claude, Cursor, or any MCP-compatible client

No more navigating multiple transit operator websites or manually parsing GTFS feeds. Your AI acts as a dedicated European travel planner and transit operations analyst.

### Who is this for?

- **Travelers** — plan multimodal journeys across French and European cities with real-time awareness
- **Urban Planners** — analyze transit accessibility, generate isochrones, and study network connectivity
- **Transit Analysts** — research operator networks, service patterns, disruptions, and schedule reliability
- **MaaS Developers** — integrate journey planning and real-time transit data into mobility applications


## Available Tools
- **get_arrivals**: Returns list of arriving services with line names and codes, origins, scheduled and real-time arrival times, platform information, delay indicators, and mode types. Essential for passenger pickup coordination, arrival monitoring, connection planning, and real-time arrival boards. AI agents use this when users ask "when does the next train arrive at this station", "show incoming services at stop X", or need to track arriving services for passenger coordination. Supports both theoretical schedules and real-time arrival predictions when operator data feeds are available.

Get upcoming arrivals at a specific transit stop
- **get_coverage**: Shows which cities and metropolitan areas are covered, data freshness indicators, and the contributing transit authorities for each region. Essential for discovering which transit networks are accessible through the API, validating region IDs for subsequent queries, understanding data coverage scope, and planning integration scope. AI agents should use this when users ask "what cities does Navitia cover", "show me all available transit regions", or need to identify the correct region ID (e.g., "fr-idf" for Paris/Ile-de-France) before making region-specific queries for lines, disruptions, or journeys.

List all available coverage regions in the Navitia platform
- **get_departures**: Returns list of departing services with line names and codes, destinations, scheduled and real-time departure times, platform or bay information, delay indicators, direction codes, and physical/commercial mode types (metro, bus, tram, RER, Transilien). Supports real-time data when available from operators. Essential for passenger information displays, departure boards, real-time transit monitoring, and journey planning. AI agents should reference this when users ask "when is the next metro from this station", "show departures from stop ID X", or need to monitor upcoming services at a known transit stop. Use data_freshness parameter to choose base_schedule (theoretical timetable) or realtime (including disruptions and delays).

Get upcoming departures from a specific transit stop
- **get_disruptions**: Returns active disruptions with affected lines, routes, stops, and networks, disruption descriptions, severity levels (minor, major, blocking), start and end timestamps, cause types (incident, maintenance, strike, weather), impact descriptions, and detour or alternative service recommendations. Covers all modes including metro, bus, tram, RER, Transilien, and regional rail across French and European networks. Essential for disruption awareness, passenger communication, journey reliability monitoring, and travel planning during service changes. AI agents should reference this when users ask "are there any disruptions on the Paris metro", "is there a strike on SNCF trains", or need to check service reliability before planning journeys.

Get active service disruptions and alerts for a transit region
- **get_isochrone**: Returns GeoJSON polygon boundaries, reachable area statistics, travel time bands, and accessibility metrics. Essential for urban planning, real estate location analysis, accessibility studies, job market research, school catchment analysis, and understanding transit connectivity. AI agents use this when users ask "what area can I reach within 30 minutes by metro from this address", "show me the accessible zone in 45 minutes by public transport", or need to analyze geographic accessibility from a specific location for housing, employment, or service planning.

Generate an isochrone map showing reachable area from a point within a time limit
- **plan_journey**: Supports combining public transit (metro, bus, tram, regional trains, high-speed rail), walking, cycling, car, bike-sharing (Vélib), and ridesharing. Returns complete itineraries with departure and arrival times, total duration, number of transfers, detailed legs with mode types, line names, operators, intermediate stops, walking distances, real-time disruption alerts, accessibility information (wheelchair access), and fare estimates. Essential for travel planning, multimodal route comparison, passenger information systems, and Mobility-as-a-Service applications across France and European cities. AI agents should use this when users ask "how do I get from Gare du Nord to Eiffel Tower", "plan a trip from Lyon Part-Dieu to Marseille", or need multimodal journey options with timing, transfers, and accessibility details. Supports traveler profiles including wheelchair, slow walker, fast walker, and luggage.

Plan a multimodal trip between two locations in France or Europe
- **get_lines**: Returns lines with codes, names, network affiliations, physical modes (metro, bus, tram, RER, rail), commercial modes, colors, text colors, route counts, and operational information. Covers metro systems (RATP Paris, TCL Lyon, TCL Marseille), bus networks, tramway systems, RER lines, Transilien suburban rail, and regional TER services across France. Essential for transit network exploration, line identification, route planning context, network analysis, and understanding service coverage by mode type. AI agents should use this when users ask "list all metro lines in Paris", "show me all tram lines in Lyon", or need line metadata to understand transit network structure and operator affiliations.

List all transit lines in a coverage region
- **get_nearby_stops**: Returns nearby objects sorted by distance with coordinates, names, types (stop point, stop area, station, address, POI), distances from search point, served lines, and administrative information. Essential for location-based transit discovery, "stops near me" features, geographic transit analysis, multimodal connection identification, and traveler navigation. AI agents use this when users ask "what metro stations are near my current location", "find transit stops within 500m of these coordinates", or need to discover accessible transit options from a specific geographic point. Supports filtering by object type (stop_point, stop_area, poi, address) and adjustable search radius.

Find transit stops near a geographic coordinate
- **get_networks**: Returns network information including names, codes, contributing authorities, coverage areas, associated lines and routes, and operational status. Covers major operators like RATP (Paris metro/bus/tram), SNCF (RER/Transilien/TER), TCL (Lyon), RTM (Marseille), TCL (Toulouse), and dozens of regional and local operators across France. Essential for operator research, network scoping, regional transit analysis, and understanding service governance structure. AI agents should reference this when users ask "what operators run transit in Paris", "list all networks in Ile-de-France", or need to identify transit operators for a specific region before querying lines or disruptions.

List all transit operators and networks in a coverage region
- **search_places**: Returns transit stops (stop areas, stop points), stations (metro, tram, bus, rail), addresses, administrative areas, and points of interest with their IDs, names, coordinates, types, and administrative information. Supports autocomplete-style search for journey planning interfaces and location discovery. Essential for stop discovery, address resolution, geocoding, journey origin/destination identification, and building location-based transit features. AI agents should use this when users ask "find the metro station near Champs-Elysees", "search for stops called Republique", or need to identify place IDs and coordinates for use in journey planning queries. Results include embedded links to departures, schedules, and nearby objects for further exploration.

Search for transit stops, stations, addresses, and POIs by name
- **get_stop_schedule**: Returns all scheduled departures with routes, destinations, first and last departure times, service frequency, headway signatures (days of operation), and physical/commercial mode information. Shows complete timetable structure including weekday, weekend, and holiday service patterns. Essential for comprehensive schedule analysis, journey planning at specific times, timetable visualization, and understanding service frequency throughout the day. AI agents should use this when users ask "show me the full timetable for this metro station", "what times does this bus run on Sundays", or need complete schedule data for a transit stop. Supports depth parameter to control level of detail in route and destination information.

Get full timetable for a specific transit stop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Navitia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a trip from Gare du Nord to the Eiffel Tower using public transit in Paris."

**🤖 AI Agent:**
> Planning multimodal journey with Navitia... I found 3 options: Option 1 (fastest): Metro Line 4 from Gare du Nord to Saint-Michel, then RER C to Champ de Mars-Tour Eiffel — 28 minutes total, 1 transfer, fare ~€2.15 with t+ ticket, departure at 09:42, arrival at 10:10. Option 2 (direct): Bus 42 from Gare du Nord to Champ de Mars — 42 minutes, no transfers, fare €2.15, departure at 09:38, arrival at 10:20. Option 3 (scenic walk): Metro Line 5 to Place d'Italie, then Line 6 (aerial) to Bir-Hakeim, 8-minute walk to Eiffel Tower — 35 minutes, 1 transfer, elevated metro segment with panoramic views. All options show normal service with no disruptions. Would you like step-by-step walking directions for any option?

---

**👤 You:**
> "Show me all metro departures from Chatelet station in the next 20 minutes."

**🤖 AI Agent:**
> Searching for Chatelet metro stops... Found multiple platforms. Fetching real-time departures: Line 1 (direction La Defense — departing in 3 minutes, on-time), Line 1 (direction Vincennes — 7 minutes, on-time), Line 4 (direction Bagneux-Lucie Aubrac — 4 minutes, on-time), Line 4 (direction Porte de Clignancourt — 9 minutes, delayed 2 minutes), Line 7 (direction Villejuif-Louis Aragon — 6 minutes, on-time), Line 7 (direction La Courneuve-8 Mai 1945 — 11 minutes, on-time), Line 11 (direction Rosny-Bois-Perrier — 8 minutes, on-time), and Line 14 (direction Aeroport d'Orly — 12 minutes, on-time). All services operated by RATP. No active disruptions on any lines. Would you like detailed route information for any specific line?

---

**👤 You:**
> "What areas can I reach within 45 minutes by public transit from Lyon Part-Dieu station?"

**🤖 AI Agent:**
> Generating isochrone from Lyon Part-Dieu with 45-minute radius (2700 seconds)... The reachable area covers most of Lyon metropolitan area including: City center (Presqu'ile) — 15 minutes by Metro A, Villeurbanne — 10 minutes by Metro A or Tram T1, Confluence district — 20 minutes by Tram T1, Gerland — 15 minutes by Metro B, Vaise — 20 minutes by Metro D, Caluire-et-Cuire — 25 minutes by Bus C, Ecully — 30 minutes by Tram T6, Bron — 30 minutes by Tram T3, Venissieux — 25 minutes by Metro D, and Oullins — 15 minutes by Metro B. Total accessible area spans approximately 12km radius. Would you like the full GeoJSON polygon for mapping, or details about accessibility to any specific neighborhood?


## Installation & Usage

To install and use the **Navitia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/navitia](https://vinkius.com/mcp/navitia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
