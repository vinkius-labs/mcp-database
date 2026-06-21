# MTA MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access NYC transit data via MTA — track subway and bus in real-time, check arrivals, monitor LIRR and Metro-North, and check service alerts from any AI agent.

## Description
Connect your **MTA API** New York City public transit data platform to any AI agent and take full control of real-time NYC Subway and MTA Bus tracking, arrival predictions, LIRR and Metro-North commuter rail monitoring, and service disruption awareness through natural conversation.

### What you can do

- **Subway Real-Time Feeds** — Access live GTFS-RT data for all NYC Subway lines with train positions and arrival predictions
- **Bus Routes** — List all MTA bus routes across Manhattan, Brooklyn, Queens, Bronx, and Staten Island
- **Bus Stops** — Get all stops for any bus route with coordinates and sequence information
- **Bus Predictions** — Get real-time estimated arrival times for any bus stop
- **Bus Vehicle Tracking** — Track real-time GPS positions of all active MTA bus vehicles
- **Service Alerts** — Monitor active disruptions across Subway, buses, LIRR, and Metro-North
- **Subway Stations** — List all 472 NYC Subway stations with coordinates, borough, and entrance data
- **LIRR Tracking** — Monitor Long Island Rail Road trains with real-time positions and arrivals
- **Metro-North Tracking** — Track Metro-North Railroad trains serving northern NYC suburbs
- **Stop-Level Bus Monitoring** — Monitor buses at specific stops with targeted arrival predictions
- **Estimated Arrivals** — Get route-filtered arrival estimates for buses at any stop
- **System Connectivity** — Verify API connectivity and synchronize timestamps

### How it works

1. Subscribe to this server
2. Enter your MTA API key (free from the Developer Portal)
3. Start tracking NYC transit from Claude, Cursor, or any MCP-compatible client

No more navigating multiple MTA apps or manually checking train and bus times. Your AI acts as a dedicated NYC transit analyst and trip planning assistant.

### Who is this for?

- **NYC Commuters** — track subway and buses, check arrivals, and monitor LIRR/Metro-North for daily commutes
- **Tourists** — navigate the NYC Subway system with station discovery and real-time arrival awareness
- **Transit Analysts** — research service patterns, vehicle positions, and system reliability across all MTA modes
- **Mobility Apps** — integrate real-time MTA data into journey planning and transit tracking applications


## Available Tools
- **get_bus_estimated_arrival**: Returns predicted arrival times, route information, destinations, wait times, and delay indicators for each expected bus. Supports both multi-route stop queries and single-route filtered queries. Essential for targeted arrival predictions, route-specific wait time estimation, and passenger trip timing. AI agents should reference this when users ask "when is the next M15 at this stop", "show arrival estimates for route B46 at stop 12345", or need route-filtered arrival data at a specific bus stop.

Get estimated arrival times for buses at a stop, optionally filtered by route
- **get_bus_predictions**: Returns predicted arrival times, route IDs, destination information, expected wait times, and whether buses are on schedule or delayed. Based on real-time vehicle tracking and schedule adherence. Essential for real-time bus arrival awareness, passenger waiting time estimation, trip timing, and connection coordination. AI agents should reference this when users ask "when is the next M15 bus at stop 12345", "show predictions for this stop", or need real-time arrival data for a specific bus stop. Stop IDs can be found using get_bus_stops.

Get next bus arrival predictions for a specific bus stop
- **get_bus_routes**: Returns route IDs, route names, operators (MTA New York City Bus, MTA Bus Company, private operators under MTA contract), and service area information. Covers local, limited-stop, and Select Bus Service (SBS) routes. Essential for route discovery, service area analysis, transit network understanding, and identifying route IDs for use in stop and prediction queries. AI agents should reference this when users ask "list all bus routes in Manhattan", "what routes serve Brooklyn", or need to identify route IDs for subsequent MTA Bus Time queries.

List all MTA bus routes in New York City
- **get_bus_stops**: Returns stop IDs (MonitoringRef), stop names, geographic coordinates (latitude, longitude), stop sequence order, and direction information. Essential for stop discovery, journey planning, accessibility mapping, and identifying stop IDs for use in arrival prediction queries. AI agents should use this when users ask "list all stops on the M15", "find bus stops along Broadway", or need to identify stop IDs for use in get_bus_predictions queries.

List all stops for a specific MTA bus route
- **get_bus_vehicle_at_stop**: Returns vehicle IDs, route IDs, current positions, expected arrival times, distances from stop, and operational status. More targeted than system-wide vehicle queries. Essential for stop-level bus tracking, passenger waiting awareness, and real-time arrival estimation at specific stops. AI agents should use this when users ask "what buses are coming to this stop", "track vehicles approaching stop 12345", or need stop-specific bus position data for passenger information.

Get buses currently at or approaching a specific bus stop
- **get_bus_vehicles**: Returns vehicle IDs, route affiliations, latitude/longitude coordinates, heading direction, speed, recorded time, and prediction availability. Covers all MTA New York City Bus and MTA Bus Company vehicles in active service. Essential for real-time bus fleet monitoring, passenger arrival estimation, route-level service awareness, and transit operations management. AI agents should use this when users ask "where are all the buses right now", "track bus positions system-wide", or need real-time vehicle position data for fleet visualization.

Get real-time positions of all active MTA bus vehicles
- **get_lirr_feed**: Returns train positions, trip updates, scheduled vs. real-time arrivals at stations, delays, track information, and service disruptions across all LIRR branches including Babylon, Ronkonkoma, Hempstead, Port Jefferson, Montauk, and more. Essential for commuter rail tracking, arrival predictions at Penn Station and Grand Central Madison, and LIRR service monitoring. AI agents should reference this when users ask "when is the next LIRR train to Penn Station", "track LIRR train positions", or need real-time commuter rail data for trip planning from Long Island into NYC.

Get real-time LIRR train data from the Long Island Rail Road
- **get_metro_north_feed**: Returns train positions, trip updates, scheduled vs. real-time arrivals, delays, track information, and service disruptions across all Metro-North lines including Hudson, Harlem, New Haven, Port Jervis, Pascack Valley, and more. Essential for commuter rail tracking, arrival predictions at Grand Central Madison, and Metro-North service monitoring. AI agents should use this when users ask "when is the next Metro-North train from White Plains", "track Metro-North positions", or need real-time commuter rail data for trip planning from Westchester, Connecticut, or the Hudson Valley into NYC.

Get real-time Metro-North Railroad train data
- **get_service_alerts**: Returns alert descriptions, affected lines and stations, severity levels, cause types (maintenance, incident, weather, special events, construction), start and end timestamps, and alternative service recommendations. Essential for service disruption awareness, alternative route planning, passenger communication, and understanding system reliability. AI agents should use this when users ask "are there any delays on the 4/5/6 line", "is LIRR running normally", or need to check service reliability before planning MTA journeys.

Get current service alerts and disruptions across the MTA system
- **get_stations**: Returns station IDs, station names, complex IDs (for multi-line stations), borough information (Manhattan, Brooklyn, Queens, Bronx, Staten Island), structure types (underground, elevated, embankment, open cut), latitude/longitude coordinates, and North/East/South/West entrance coordinates. Essential for station discovery, rail network mapping, route planning, and identifying station codes for use in journey planning queries. AI agents should use this when users ask "list all stations in Manhattan", "what is the station code for Times Square", or need to understand the NYC Subway network geography.

List all NYC Subway stations with details
- **get_subway_feed**: Supports feed IDs grouped by line: "1" (lines 1,2,3,4,5,6,S), "2" (lines A,C,E), "3" (lines B,D,F,M), "4" (lines G), "5" (lines J,Z), "6" (lines N,Q,R,W), "7" (lines L), "11" (Staten Island Railway), "16" (Shuttle 42nd St), "21" (Shuttle Franklin Ave), "26" (Shuttle Rockaway Park). Returns train positions, trip updates, scheduled vs. real-time arrivals, delays, and service disruptions. Essential for real-time subway tracking, arrival predictions, and service monitoring across the entire NYC Subway system. AI agents should use this when users ask "when is the next 1 train", "show real-time positions for the A line", or need live subway data for trip planning. Feed IDs are required and can be found in MTA documentation.

Get real-time subway feed data for specific NYC Subway lines
- **get_system_time**: Returns the official server timestamp in ISO 8601 format. Useful for synchronizing local clocks with the MTA system, verifying API connectivity, testing authentication, and timestamp alignment for real-time data correlation. AI agents should use this as a connectivity check before making more complex queries, or when users need to verify API responsiveness and authentication validity.

Get the current MTA Bus Time system timestamp


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MTA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the next trains on the 1/2/3 line."

**🤖 AI Agent:**
> Fetching subway feed for lines 1/2/3/4/5/6/S (feed ID: 1)... Real-time GTFS-RT data shows: 1 Train to Van Cortlandt Park — 3 stops away, arriving in 4 minutes; 2 Train to Wakefield-241st — 5 stops away, arriving in 7 minutes; 3 Train to Harlem-148th St — 8 stops away, arriving in 11 minutes. All trains currently running on or close to scheduled times with no major delays reported. Would you like predictions for a specific station?

---

**👤 You:**
> "When is the next M15 bus arriving at the stop near 14th Street and 3rd Avenue?"

**🤖 AI Agent:**
> Looking up M15 route stops... Found stop ID 308238 at 14 St/3 Av. Checking real-time predictions: M15 Select Bus Service southbound to South Ferry — arriving in 2 minutes; M15 local southbound — arriving in 8 minutes; M15 SBS northbound to East Harlem — arriving in 12 minutes. All vehicles currently on schedule. The SBS stop requires fare payment at street-level machines before boarding. Would you like me to track the exact GPS positions of these buses?

---

**👤 You:**
> "Check if there are any service alerts affecting the LIRR right now."

**🤖 AI Agent:**
> Checking MTA service alerts... Currently 2 active LIRR alerts: 1) Babylon Branch — Trains experiencing 10-15 minute delays due to earlier signal problem at Jamaica. Normal service expected to resume by 6:30 PM. 2) Port Jefferson Branch — Track work in effect between Huntington and Northport, expect single-tracking with 20 minute delays through 11:00 PM tonight. All other LIRR branches running on schedule. Penn Station and Grand Central Madison terminals operating normally. Would you like me to check specific train predictions for your branch?


## ❓ FAQ

**Q: Can my AI check when the next subway train is arriving at my station?**
Yes! Use the `get_subway_feed` tool with the appropriate feed ID for your line. Feed IDs are grouped: "1" covers lines 1,2,3,4,5,6,S; "2" covers A,C,E; "3" covers B,D,F,M; "4" is G; "5" is J,Z; "6" covers N,Q,R,W; "7" is L; "11" is Staten Island Railway. This returns real-time GTFS-RT data with train positions, trip updates, scheduled vs. real-time arrivals, and delay information. For station-level predictions, combine with `get_stations` to find your station code first.

**Q: How do I check when the next MTA bus is arriving at a specific stop?**
First use `get_bus_stops` with a route ID to find the stop ID (MonitoringRef) for your location. Then use `get_bus_predictions` with that stop ID to get real-time estimated arrival times, route information, destinations, and delay indicators. For more targeted predictions, use `get_bus_estimated_arrival` which allows filtering by both stop ID and route ID. Stop IDs are numeric identifiers assigned by MTA to each physical bus stop across NYC.

**Q: Are there any service disruptions affecting my subway line or bus route right now?**
Use `get_service_alerts` to check all active service disruptions across the MTA system. This returns alerts with affected lines and stations, disruption descriptions, severity levels, cause types (maintenance, incident, weather, special events, construction), start and end timestamps, and alternative service recommendations. Covers NYC Subway, buses, LIRR, and Metro-North. Always check this before planning any journey to ensure you are aware of delays, planned work, or service changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mta](https://vinkius.com/mcp/mta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MTA** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MTA** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mta": {
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
