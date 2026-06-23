# TransportAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transportapi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access UK public transport data via TransportAPI — track buses and trains, plan journeys, check departures, and monitor service disruptions from any AI agent.

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


## Available Tools (12)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TransportAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all bus departures from Oxford Circus in the next 30 minutes."

**🤖 AI Agent:**
> Searching for Oxford Circus bus stops... Found stop ID 490007653. Fetching real-time departures: I found 8 buses departing in the next 30 minutes: Route 94 (towards Piccadilly Circus, departing in 2 minutes, on-time), Route 159 (towards Streatham, 5 minutes, delayed 3 minutes), Route 453 (towards Deptford Bridge, 8 minutes, on-time), Route 13 (towards Euston, 12 minutes, on-time), Route 88 (towards Clapham Common, 15 minutes, on-time), Route 113 (towards Edgware, 18 minutes, delayed 5 minutes), Route 94 (towards Acton Green, 22 minutes, on-time), and Route 12 (towards Dulwich Library, 27 minutes, on-time). All services operated by Transport for London. Would you like more details about any specific route?

---

**👤 You:**
> "What trains are departing from London Paddington to Bristol in the next 2 hours?"

**🤖 AI Agent:**
> Fetching rail departures from Paddington (PAD)... I found 6 direct services to Bristol Temple Meads (BRI) in the next 2 hours: GWR 10:15 (arriving 11:52, 1h 37m, Platform 8, on-time), GWR 10:45 (arriving 12:24, 1h 39m, Platform 10, delayed 4 minutes), GWR 11:15 (arriving 12:51, 1h 36m, Platform 8, on-time), GWR 11:32 (arriving 13:14, 1h 42m, Platform 12, on-time), GWR 11:45 (arriving 13:26, 1h 41m, Platform 10, on-time), and GWR 12:02 (arriving 13:41, 1h 39m, Platform 8, on-time). All services operated by Great Western Railway with modern IEP trains. Fastest journey time is 1h 36m. Would you like me to check the calling points for any specific service?

---

**👤 You:**
> "Plan a journey from Manchester Airport to the city centre using public transport."

**🤖 AI Agent:**
> Planning multimodal journey with TransportAPI... I found 3 options: Option 1 (fastest): Train from Manchester Airport to Manchester Piccadilly — 18 minutes, TransPennine Express or Northern Rail, trains every 10 minutes, fare from £3.50 with contactless, arrive at Piccadilly Gardens in 25 minutes total. Option 2 (direct bus): Metrolink tram from Airport to St Peters Square — 35 minutes, direct service every 12 minutes, fare £3.30 with contactless. Option 3 (budget): Bus 43 from Airport Terminal to Piccadilly Gardens — 55 minutes, Stagecoach service, fare £2.00 with contactless cap. All options show normal service with no disruptions. Would you like real-time departures for any option?


## ❓ FAQ

**Q: Can my AI check when the next bus is arriving at a specific UK bus stop?**
Yes! First use `search_stops` to find the bus stop by name or location (e.g., "Oxford Street" or "Piccadilly Circus"). This returns the Naptan stop ID. Then use `get_bus_departures` with that stop ID to see all upcoming departures with expected arrival times, line numbers, destinations, and any delay information. You can also use `get_bus_arrivals` to monitor incoming services. The API provides real-time predictions based on live vehicle tracking across Great Britain.

**Q: How do I plan a complete journey from my hotel to a UK attraction using public transport?**
Use the `get_journey_plan` tool with your hotel address or postcode as the origin and the attraction name or postcode as the destination. The TransportAPI journey planner will return complete multimodal itineraries combining buses, trains, trams, underground (tube), walking, and cycling with departure times, arrival times, total duration, number of changes, detailed legs with line names and operators, walking distances, and real-time disruption alerts. You can also specify a desired departure or arrival time for time-specific planning.

**Q: Can I check if there are any disruptions or engineering works affecting UK rail services?**
Absolutely! Use `get_updates` to fetch current service alerts and disruption notices across the UK transport network. You can filter by mode ("rail" for trains, "bus" for buses) to get targeted alerts. The results include affected lines or stations, disruption descriptions, severity levels, expected duration, and alternative route recommendations. For station-specific information, use `get_rail_departures` or `get_rail_arrivals` which include cancellation and delay indicators for individual services.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transportapi](https://vinkius.com/mcp/transportapi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TransportAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transportapi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TransportAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transportapi": {
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
