# LA Metro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/la-metro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access Los Angeles Metro data via API — track buses and rail in real-time, check arrivals, plan rail trips, and monitor service alerts from any AI agent.

## Description
Connect your **LA Metro API** Los Angeles public transit data platform to any AI agent and take full control of real-time Metrobus and Metro Rail tracking, arrival predictions, rail-to-rail journey planning, and service disruption monitoring through natural conversation.

### What you can do

- **Metrobus Stops** — List all bus stops system-wide or filtered by route with coordinates and service messages
- **Metrobus Routes** — Browse all Metrobus routes including local, rapid, and express services across LA County
- **Bus Schedules** — Get complete schedule data with run patterns and stop sequences for any bus route
- **Bus Vehicle Tracking** — Track real-time GPS positions of all active Metrobus vehicles
- **Stop Predictions** — Get next bus arrival predictions for any specific bus stop with minutes and seconds
- **Metro Rail Stations** — List all rail stations across B (Red), D (Purple), A (Blue), E (Expo), C (Green), and K lines
- **Rail Arrivals** — Get next train arrival predictions at any Metro Rail station with line and destination info
- **Rail-to-Rail Planning** — Plan rail-only journeys between any two Metro Rail stations with transfer guidance
- **Rail Routes** — Browse all Metro Rail lines with colors, station counts, and operational metadata
- **Service Alerts** — Monitor active disruptions across Metro Rail and Metrobus with severity and alternatives
- **Rail Vehicle Positions** — Track real-time positions of Metro Rail trains across the network
- **Bus Locations** — Get real-time bus locations system-wide or filtered by specific route

### How it works

1. Subscribe to this server
2. Enter your LA Metro API key (if required — many endpoints are open data)
3. Start tracking LA Metro transit from Claude, Cursor, or any MCP-compatible client

No more navigating the Metro website or manually checking train and bus times. Your AI acts as a dedicated LA transit analyst and trip planning assistant.

### Who is this for?

- **LA Commuters** — track buses and rail, check arrivals, and plan rail-only trips across LA County
- **Tourists** — navigate the Metro Rail system with station discovery and rail-to-rail journey planning
- **Transit Analysts** — research service patterns, vehicle positions, and system reliability
- **Mobility Apps** — integrate real-time LA Metro data into journey planning and transit tracking applications


## Available Tools
- **get_bus_locations**: Returns vehicle IDs, route IDs, latitude/longitude coordinates, heading direction, seconds since last report, predictability indicators, and trip/run identifiers. Can query all buses system-wide or filter by specific route ID for targeted route-level tracking. Essential for real-time bus fleet monitoring, passenger arrival estimation, route-level service awareness, and transit operations management. AI agents should reference this when users ask "show me all buses on route 720", "where are the active buses right now", or need real-time bus position data for fleet visualization or arrival prediction.

Get real-time bus locations system-wide or for a specific route
- **get_bus_routes**: Returns route IDs, route names, types (local, rapid, express, Metro Rail link), direction listings, and route metadata. Covers hundreds of routes serving the entire LA Metro service area including downtown LA, Hollywood, Santa Monica, San Fernando Valley, South Bay, East LA, and beyond. Essential for route discovery, service area analysis, transit network understanding, and identifying route IDs for use in stop and schedule queries. AI agents should reference this when users ask "list all Metrobus routes", "what routes serve downtown LA", or need to identify route IDs for subsequent Metrobus queries.

List all Metrobus routes in the LA Metro system
- **get_bus_schedule**: Returns run IDs, direction information (inbound/outbound, eastbound/westbound), stop sequences, and scheduled timing data. Essential for schedule analysis, journey planning at specific times, understanding route direction patterns, and passenger trip preparation. AI agents should use this when users ask "show me the schedule for route 720", "what are the run patterns for the 4 line", or need detailed schedule data for a specific bus route to plan trips at specific times.

Get the schedule for a specific Metrobus route
- **get_bus_stops**: Returns stop IDs, names, geographic coordinates (latitude, longitude), route affiliations, and any service messages or alerts associated with each stop. Essential for stop discovery, journey planning, accessibility mapping, and understanding bus network geography across Los Angeles County. AI agents should use this when users ask "list all stops on the 720 Rapid", "find bus stops near Union Station", or need to identify stop IDs for use in prediction queries. If no route_id is provided, returns all stops system-wide.

List all Metrobus stops or stops on a specific bus route
- **get_bus_vehicles**: Returns vehicle IDs, route affiliations, latitude/longitude coordinates, heading direction, seconds since last report, predictability indicators (whether the vehicle is running on predicted schedule or actual GPS), and run/trip identifiers. Essential for real-time bus tracking, passenger wait time estimation, bus arrival prediction, and fleet monitoring. AI agents should use this when users ask "where are the buses right now", "track vehicle 1234", or need to locate specific Metrobus vehicles for real-time arrival awareness.

Get real-time locations of active Metrobus vehicles
- **get_rail_arrivals**: Returns predicted arrival times, train destination names, line colors (Red, Purple, Blue, Expo, Green, Gold, K), direction indicators, and train run identifiers. Essential for real-time rail arrival awareness, passenger waiting time estimation, connection planning, and station-level trip timing. AI agents should reference this when users ask "when is the next Red Line train at Union Station", "show upcoming trains at 7th Street/Metro Center", or need station-specific Metro Rail arrival predictions. Station IDs can be found using get_rail_stations.

Get next train arrival predictions at a specific Metro Rail station
- **get_rail_vehicle_positions**: Returns train identifiers, line affiliations, latitude/longitude coordinates, heading direction, run/trip IDs, and prediction status. Essential for real-time rail tracking, train location awareness, and understanding train distribution across the network. AI agents should use this when users ask "where are the Red Line trains right now", "track train positions on the Expo Line", or need to visualize train locations for operational monitoring or passenger information.

Get real-time positions of Metro Rail trains
- **get_rail_routes**: Essential for line identification, rail network understanding, service area analysis, and identifying line IDs for use in rail journey planning. AI agents should reference this when users ask "list all Metro Rail lines", "what lines does Metro operate", or need line metadata for rail network context.

List all Metro Rail lines and routes
- **get_rail_stations**: Returns station IDs, names, display names, geographic coordinates (latitude, longitude), line affiliations, station order on each line, cross streets, and accessibility information. Essential for station discovery, rail network mapping, route planning, and identifying station IDs for use in arrival and rail-to-rail queries. AI agents should use this when users ask "list all stations on the Red Line", "what is the station code for 7th Street/Metro Center", or need to understand the Metro Rail network geography.

List all Metro Rail stations with details
- **get_rail_to_rail**: Returns recommended routes, transfer stations, estimated travel times, number of transfers, line sequences, and step-by-step rail directions. Essential for rail trip planning, transfer identification, travel time estimation, and understanding rail connectivity across the Metro network. AI agents should use this when users ask "how do I get from North Hollywood to Santa Monica by rail", "plan a rail trip from Union Station to LAX", or need rail-only journey planning between two Metro Rail stations. Station IDs can be found using get_rail_stations.

Get rail-to-rail journey planning between two Metro Rail stations
- **get_service_alerts**: Returns alert descriptions, affected routes and stations, severity levels, start and end timestamps, cause types (maintenance, incident, weather, special events), and alternative service recommendations. Essential for service disruption awareness, alternative route planning, passenger communication, and understanding system reliability. AI agents should use this when users ask "are there any delays on the Red Line", "is Metro running normally today", or need to check service reliability before planning Metro journeys.

Get current service alerts and disruptions across the LA Metro system
- **get_stop_predictions**: Returns predicted arrival times in minutes and seconds, route IDs, run IDs, direction information, departure indicators, and prediction confidence levels. Essential for real-time bus arrival awareness, passenger waiting time estimation, trip timing, and connection coordination. AI agents should reference this when users ask "when is the next bus at stop 5678", "show predictions for this stop", or need real-time arrival data for a specific bus stop. Stop IDs can be found using get_bus_stops.

Get next bus arrival predictions for a specific bus stop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LA Metro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all Metrobus stops on the 720 Rapid route."

**🤖 AI Agent:**
> Fetching stops for Route 720 Rapid... I found 76 stops along this east-west rapid corridor. Key stops include: Atlantic Station (East end), Indiana Street, Soto Street, Boyle Heights, 1st/Main, Civic Center, Grand Avenue, Westlake/MacArthur Park, Wilshire/Vermont, Wilshire/Normandie, Wilshire/Western, Koreatown, Miracle Mile, Beverly Hills, Century City, Westwood/UCLA, and Santa Monica Blvd/Westwood (West end). Would you like predictions for a specific stop?

---

**👤 You:**
> "What are the next Red Line trains arriving at Union Station?"

**🤖 AI Agent:**
> Fetching Red Line arrivals at Union Station (station 80222)... Next trains: North Hollywood — 3 minutes, 6 cars; North Hollywood — 11 minutes, 6 cars; North Hollywood — 19 minutes, 6 cars. All Red Line trains operating on schedule with no service alerts. Trains run approximately every 8 minutes during peak hours. Would you like me to check rail-to-rail connections from Union Station to your destination?

---

**👤 You:**
> "Plan a rail journey from North Hollywood to Santa Monica."

**🤖 AI Agent:**
> Planning rail-to-rail journey... Recommended route: Take B Line (Red) from North Hollywood to 7th Street/Metro Center — 26 minutes. Transfer to E Line (Expo) at 7th Street/Metro Center heading westbound to Downtown Santa Monica — 32 minutes. Total journey time: approximately 58 minutes plus transfer time. 1 transfer required. Both lines running on schedule. Would you like me to check next train times at North Hollywood station?


## ❓ FAQ

**Q: Can my AI check when the next Metrobus is arriving at a specific stop in LA?**
Yes! First use `get_bus_stops` with a route_id to find the stop ID for your location. Then use `get_stop_predictions` with that stop ID to get real-time arrival predictions in minutes and seconds, including route numbers, direction, and whether the bus is departing soon. This gives you live predictions based on actual vehicle GPS positions and schedule adherence.

**Q: How do I plan a Metro Rail journey from one station to another?**
Use `get_rail_stations` first to find the station IDs for your origin and destination. Then use `get_rail_to_rail` with both station IDs to get the recommended rail route with transfer stations, estimated travel time, number of transfers, and step-by-step directions. You can also use `get_rail_arrivals` at your origin station to see when the next trains are coming.

**Q: Are there any service disruptions affecting Metro Rail or Metrobus right now?**
Use `get_service_alerts` to check all active service disruptions across the LA Metro system. This returns alerts with affected routes and stations, disruption descriptions, severity levels, cause types (maintenance, incident, weather, special events), start and end times, and alternative service recommendations. Check this before planning any journey to ensure you are aware of delays or service changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/la-metro](https://vinkius.com/mcp/la-metro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LA Metro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `la-metro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LA Metro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "la-metro": {
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
