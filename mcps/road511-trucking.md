# Road511 Trucking MCP Server

Access trucking data via Road511 — track truck routes, bridge clearances, weigh stations, truck stops, parking, and weight restrictions across US and Canada from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/road511-trucking)

## Overview
**Category:** shipping-logistics
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Road511 Trucking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/road511-trucking](https://vinkius.com/mcp/road511-trucking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
