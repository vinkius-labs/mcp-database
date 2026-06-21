# Lyko MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lyko)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

Access European public transit via Lyko — plan intermodal trips, check departures, search stops, and monitor transit operators from any AI agent.

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


## Available Tools (12)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lyko** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a trip from Paris Gare du Nord to the Palace of Versailles using public transit."

**🤖 AI Agent:**
> Planning multimodal route with Lyko... I found 3 options: Option 1 (fastest): RER C from Gare d'Austerlitz to Versailles Rive Gauche — 52 minutes total, 1.2km walk from Gare du Nord to departure station, arrive at 10:23, fare €3.65. Option 2 (convenient): SNCF Transilien Line N from Gare Saint-Lazare to Versailles Rive Droite — 48 minutes, 2.1km walk to departure, depart at 09:54, arrive at 10:42, fare €3.65. Option 3 (scenic): Metro Line 6 to Bir-Hakeim, then RER C to Versailles — 68 minutes with 1 transfer, fare €3.65. All options show normal service with no delays. Would you like detailed step-by-step directions for any option?

---

**👤 You:**
> "Show me all departures from Berlin Alexanderplatz station in the next 30 minutes."

**🤖 AI Agent:**
> Fetching real-time departures for Berlin Alexanderplatz... I found 23 departures in the next 30 minutes across multiple lines: S-Bahn S5 (toward Strausberg Nord, departing in 3 minutes, Platform 4, on-time), S-Bahn S7 (toward Ahrensfelde, 7 minutes, Platform 3, on-time), U-Bahn U2 (toward Ruhleben, 5 minutes, Platform B2, on-time), U-Bahn U5 (toward Hauptbahnhof, 9 minutes, Platform B1, on-time), U-Bahn U8 (toward Wittenau, 12 minutes, Platform C1, delayed 4 minutes), Tram M4 (toward Zingster Strasse, 6 minutes, Platform A, on-time), Tram M5 (toward Virchow-Klinikum, 15 minutes, Platform B, on-time), Bus 100 (toward Zoologischer Garten, 11 minutes, Platform D, on-time), and 15 more services. Would you like filtering by specific line or direction?

---

**👤 You:**
> "What transit operators are available in the Netherlands, and is NS (Dutch Railways) running normally today?"

**🤖 AI Agent:**
> Checking Netherlands transit operators... I found 8 operators: NS (Nederlandse Spoorwegen) — national rail network, GVB — Amsterdam public transport (metro, tram, bus), RET — Rotterdam metro and tram, HTM — The Hague transit, Arriva — regional buses and trains, Connexxion — regional buses, Breng — Arnhem-Nijmegen regional transit, and Qbuzz — Groningen-Drenthe buses. Now checking NS network status: NS is operating normally today with all major intercity lines running on schedule. No reported disruptions, strikes, or planned works affecting main routes. Minor delays of 2-3 minutes on regional services in the Limburg area due to maintenance. High-speed international services (Thalys, Eurostar to London) are also running normally. Would you like me to check any other operator?


## ❓ FAQ

**Q: Can my AI plan a complete multimodal trip from my hotel to a tourist attraction using public transit?**
Yes! Use the `plan_trip` tool with your hotel address or name as the origin and the tourist attraction as the destination. The Lyko routing engine will return complete door-to-door itineraries combining buses, trains, subways, trams, and walking segments with departure times, arrival times, total duration, number of transfers, line names, operators, walking distances, and real-time delay information. You can also specify preferred transport modes or a desired departure time. Perfect for tourist planning, business travel, and navigating unfamiliar European cities.

**Q: How do I check real-time departures and arrivals at a specific train station or bus stop?**
First, use `search_stops` to find the stop by name (e.g., "Gare du Nord" or "Alexanderplatz"). Once you have the stop ID, use `get_departures` to see upcoming services with ETAs, platforms, and delay indicators, or `get_arrivals` to track incoming services. The results include line names, destinations, scheduled vs. real-time times, and operator information. This is perfect for passenger pickup coordination, connection planning, and monitoring service reliability.

**Q: Can I check if there are any service disruptions or strikes affecting transit operators in France or Germany?**
Absolutely! Use `get_operators` with the country filter (e.g., "FR" for France, "DE" for Germany) to list all available operators, then use `get_network_status` with the operator ID (e.g., "sncf" for SNCF, "db" for Deutsche Bahn) to check current service disruptions, planned works, strike notifications, weather impacts, and line closures. This gives you real-time awareness of transit reliability across 300+ European operators. AI agents can proactively alert travelers to service issues before trip planning.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lyko](https://vinkius.com/mcp/lyko)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lyko** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lyko` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lyko** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lyko": {
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
