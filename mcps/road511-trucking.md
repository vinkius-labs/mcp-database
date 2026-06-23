# Road511 Trucking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/road511-trucking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shipping-logistics](../categories/shipping-logistics.md)

Access trucking data via Road511 — track truck routes, bridge clearances, weigh stations, truck stops, parking, and weight restrictions across US and Canada from any AI agent.

## Description
Connect your **Road511 Trucking API** to any AI agent and take full control of North American truck route planning, bridge clearance verification, weigh station awareness, truck stop discovery, and weight restriction monitoring through natural conversation.

### What you can do

- **STAA Truck Routes** — Access 479,000+ STAA-designated truck route segments and NHFN freight corridors
- **Bridge Clearances** — Query 621,000+ National Bridge Inventory records for vertical clearance heights
- **Weight Restrictions** — Monitor seasonal and permanent weight restrictions across all jurisdictions
- **Truck Stops** — Find truck stops and travel plazas with fuel, amenities, and parking information
- **Truck Parking** — Locate truck parking facilities with availability data for HOS compliance planning
- **Weigh Stations** — Track weigh station locations, hours, and bypass program participation
- **Rest Areas** — Find rest areas and driver facilities along major highway corridors
- **Truck Incidents** — Monitor traffic incidents, construction, and closures affecting truck routes
- **System Health** — Check API health and data source status across 65 jurisdictions

### How it works

1. Subscribe to this server
2. Enter your Road511 API key (free 14-day trial available)
3. Start monitoring trucking data from Claude, Cursor, or any MCP-compatible client

No more navigating multiple state 511 websites or manually checking truck route compliance. Your AI acts as a dedicated trucking analyst and route planning assistant.

### Who is this for?

- **Fleet Dispatchers** — plan compliant routes, check bridge clearances, and locate truck stops and parking
- **Owner-Operators** — find weigh stations, rest areas, and monitor weight restrictions before trips
- **Logistics Planners** — analyze freight corridors, track disruptions, and optimize truck routing
- **Safety Managers** — verify bridge clearances, monitor incidents, and ensure weight compliance


## Available Tools (10)
- **get_bridge_clearances**: Returns bridge location coordinates, clearance height in feet/meters, bridge identifier, road name, and jurisdiction. Supports filtering by jurisdiction, bounding box, and radius search. Essential for truck height compliance planning, low bridge avoidance, oversized load routing, and fleet safety management. AI agents should use this when users ask "find low bridges under 14 feet on I-95", "what bridge clearances exist in this area", or need vertical clearance data for truck route planning.

Get bridge clearance heights from the National Bridge Inventory for truck route planning
- **get_trucking_health**: Returns API availability, response times, data source connectivity per jurisdiction, last update timestamps, and system alerts. Essential for monitoring API reliability, verifying data freshness, troubleshooting integration issues, and ensuring production system uptime. AI agents should use this as a diagnostic tool when users report missing trucking data, when debugging integration issues, or as a periodic health check before making complex trucking data queries.

Check API health and trucking data source status
- **get_rest_areas**: Returns facility names, locations, available amenities (restrooms, vending, picnic areas, pet areas, RV/truck parking), operating hours, and jurisdiction. Supports filtering by jurisdiction, bounding box, and radius search. Essential for driver rest planning, HOS compliance stops, facility identification along routes, and driver comfort services. AI agents should reference this when users ask "show rest areas along I-90 in Montana", "find rest stops with truck parking near this point", or need rest area data for driver scheduling and route planning.

Get rest areas and driver facilities along highways across US and Canada
- **get_trucking_summary**: Returns counts of truck routes, bridge clearances, weigh stations, truck stops, parking facilities, active incidents, and data source status. Essential for data coverage awareness, system health monitoring, and understanding data availability by region. AI agents should use this when users ask "how many truck stops are in the system", "is the Texas weigh station data current", or need a system-wide overview of trucking data quality and coverage.

Get summary statistics and data source health for trucking data across all jurisdictions
- **get_truck_incidents**: Returns incident type, severity, affected roads, start and end times, descriptions, detour information, and geometry. Supports filtering by jurisdiction, road name, severity, status, and geographic area. Essential for route disruption awareness, detour planning, delivery time estimation, and freight safety. AI agents should use this when users ask "show incidents affecting truck routes in Illinois", "is there construction on I-80 in Pennsylvania", or need current traffic incident data for truck route planning.

Get traffic incidents affecting truck routes including closures, construction, and advisories
- **get_truck_parking**: Returns parking facility names, locations, capacity information, real-time availability (where available), amenity details, and jurisdiction. Supports filtering by jurisdiction, bounding box, and radius search. Essential for Hours of Service (HOS) compliance planning, rest stop scheduling, parking shortage awareness, and safe stopping location identification. AI agents should reference this when users ask "where can I park my truck near Chicago", "show truck parking availability along I-70", or need parking location data for HOS-compliant route planning.

Get truck parking availability and locations across US and Canada
- **get_truck_routes**: Returns route geometry, jurisdiction, route designation, and descriptive information. Supports filtering by jurisdiction (state/province), bounding box, and radius search from coordinates. Essential for truck route planning, freight corridor analysis, compliance verification, and logistics routing. AI agents should use this when users ask "show me STAA truck routes in California", "find NHFN corridors in Texas", or need official truck-designated highway data for route planning and compliance.

Get STAA truck routes and NHFN freight corridors across US and Canada
- **get_truck_stops**: Returns stop names, addresses, coordinates, available services (fuel, food, showers, repair), and operating hours. Supports filtering by jurisdiction, bounding box, and radius search. Essential for trip planning, fuel stop scheduling, driver rest planning, and freight corridor services identification. AI agents should use this when users ask "find truck stops along I-80 in Iowa", "show travel plazas within 50 miles of this point", or need truck stop locations for route planning and driver scheduling.

Get truck stops and travel plazas across US and Canada for trip planning
- **get_weigh_stations**: Returns station names, locations, operating hours, bypass program participation (PrePass, Drivewyze, NORPASS), open/closed status, and jurisdiction. Supports filtering by jurisdiction, bounding box, and radius search. Essential for compliance planning, bypass program routing, weigh stop scheduling, and weight inspection awareness. AI agents should use this when users ask "show weigh stations on I-5 in Oregon", "are there open weigh stations near this location", or need weigh station data for route planning and compliance management.

Get weigh station locations and status across US and Canada
- **get_weight_restrictions**: Returns restriction details including affected roads, weight limits, effective dates, restriction type (seasonal, permanent, temporary), severity, and jurisdiction. Supports filtering by jurisdiction, road name, severity, and geographic area. Essential for weight compliance verification, seasonal route planning, load planning, and avoiding weight violation fines. AI agents should reference this when users ask "are there seasonal weight restrictions in Minnesota right now", "show weight limits on this route", or need current weight restriction data for freight planning.

Get truck weight restrictions including seasonal restrictions across US and Canada


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Road511 Trucking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all weigh stations on I-5 in Oregon and their current status."

**🤖 AI Agent:**
> Querying weigh stations on I-5 in Oregon... Found 5 weigh stations: Northbound I-5 Milepost 438 (Ashland) — Open 24/7, PrePass and Drivewyze enabled. Southbound I-5 Milepost 437 (Ashland) — Open 6AM-10PM, Drivewyze enabled. Northbound I-5 Milepost 285 (Eugene) — Open 24/7, all bypass programs. Southbound I-5 Milepost 284 (Eugene) — Currently closed for maintenance, reopening at 6AM. Northbound I-5 near Salem — Open 24/7, all bypass programs. Would you like bypass program details for any station?

---

**👤 You:**
> "Find truck stops with parking within 30 miles of Des Moines, Iowa."

**🤖 AI Agent:**
> Searching truck stops near Des Moines, IA (lat: 41.5868, lon: -93.6250) within 30 miles... Found 8 truck stops: TA Travel Center — I-80 Exit 135, 85 parking spaces, fuel, showers, restaurant, open 24/7. Pilot Flying J — I-35 Exit 83, 62 spaces, fuel, showers, laundry, open 24/7. Love's Travel Stop — I-80 Exit 129, 48 spaces, fuel, dog wash, open 24/7. Petro Stopping Center — I-235 Exit 3B, 55 spaces, full service, open 24/7. Plus 4 additional stops with 20-40 spaces each. All locations have real-time parking availability. Would you like current availability counts for any location?

---

**👤 You:**
> "Show me STAA truck routes and any active incidents affecting trucking in Illinois."

**🤖 AI Agent:**
> Fetching STAA truck routes for Illinois... Found 12,450 route segments covering I-80, I-55, I-57, I-70, I-74, I-90, I-94, and major US highways. Active incidents affecting trucking: I-80 westbound at Mile 142 — Lane closure due to construction, expect 20-minute delays, detour via IL-47. I-55 southbound at Bloomington — Accident cleared, residual delays 10-15 minutes. I-294 northbound — Weight restriction in effect for trucks over 80,000 lbs due to bridge maintenance, ends at 5PM today. All other major truck routes operating normally.


## ❓ FAQ

**Q: Can my AI check for low bridges on a truck route in California?**
Yes! Use the `get_bridge_clearances` tool with jurisdiction=CA to get all bridge clearance data for California. You can also filter by bounding box or radius from specific coordinates. The API returns bridge locations, clearance heights in feet, bridge identifiers, and road names. This is essential for truck height compliance planning and avoiding low-bridge incidents.

**Q: How do I find truck parking near a specific location for HOS compliance?**
Use the `get_truck_parking` tool with lat, lon, and radius parameters to find truck parking facilities near your current location. For example: lat=41.8781, lon=-87.6298, radius=50 finds parking within 50km of Chicago. Results include facility names, coordinates, capacity information, and amenity details. This is critical for Hours of Service (HOS) compliance planning and safe rest stop identification.

**Q: Are there any seasonal weight restrictions affecting my route right now?**
Use the `get_weight_restrictions` tool with jurisdiction and status=active to find all current weight restrictions in a state or province. You can also filter by specific road name (e.g., road=I-94) to check restrictions on a particular highway. Returns restriction details, weight limits, effective dates, and affected road segments. Essential for avoiding weight violation fines and planning compliant loads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/road511-trucking](https://vinkius.com/mcp/road511-trucking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Road511 Trucking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `road511-trucking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Road511 Trucking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "road511-trucking": {
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
