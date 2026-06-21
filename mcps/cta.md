# CTA MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cta)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cta-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cta-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access Chicago transit data via CTA — track L trains and buses in real-time, check arrivals, monitor service alerts, and plan trips from any AI agent.

## Description
Connect your **CTA API** Chicago public transit data platform to any AI agent and take full control of real-time L train and CTA Bus tracking, arrival predictions, service disruption monitoring, and route status awareness through natural conversation.

### What you can do

- **L Train Arrivals** — Get real-time arrival predictions for any CTA L station with train destinations and line colors
- **L Train Positions** — Track live positions of all active trains system-wide or filtered by line (Red, Blue, Brown, Green, Orange, Purple, Pink, Yellow)
- **Bus Predictions** — Get estimated arrival times for any CTA bus stop with route and destination info
- **Bus Vehicle Tracking** — Track real-time GPS positions of all active CTA buses system-wide or by route
- **Bus Routes** — List all CTA bus routes across Chicago neighborhoods
- **Bus Stops** — Get all stops for any bus route with coordinates and direction information
- **Service Alerts** — Monitor active disruptions across L trains and buses with severity and alternatives
- **Route Status** — Quick system-wide health check showing which lines are running on-time or delayed
- **Stop Details** — Get detailed location info for any CTA bus stop
- **Route Directions** — Understand direction patterns (northbound, southbound) for any bus route
- **System Connectivity** — Verify API connectivity and synchronize timestamps

### How it works

1. Subscribe to this server
2. Enter your CTA Train Tracker API key and CTA Bus Tracker API key (both free from the Developer Portal)
3. Start tracking Chicago transit from Claude, Cursor, or any MCP-compatible client

No more navigating multiple CTA apps or manually checking train and bus times. Your AI acts as a dedicated Chicago transit analyst and trip planning assistant.

### Who is this for?

- **Chicago Commuters** — track L trains and buses, check arrivals, and monitor service alerts for daily commutes
- **Tourists** — navigate the CTA L system with station discovery and real-time arrival awareness
- **Transit Analysts** — research service patterns, vehicle positions, and system reliability across CTA modes
- **Mobility Apps** — integrate real-time CTA data into journey planning and transit tracking applications


## Available Tools
- **get_bus_predictions**: Returns predicted arrival times in minutes and seconds, route IDs, destination descriptions, vehicle IDs, block IDs, trip designators, and whether buses are scheduled or real-time tracked. Based on real-time vehicle tracking and schedule adherence. Essential for real-time bus arrival awareness, passenger waiting time estimation, trip timing, and connection coordination. AI agents should use this when users ask "when is the next 22 Clark bus at stop 1234", "show predictions for this stop", or need real-time arrival data for a specific CTA bus stop. Stop IDs can be found using get_bus_stops.

Get next bus arrival predictions for a specific CTA bus stop
- **get_bus_routes**: Returns route IDs, short names (e.g., "22", "36"), long names (e.g., "22-Clark", "36-Broadway"), route colors, and route directions. Covers local, limited-stop, and express services across all Chicago neighborhoods. Essential for route discovery, service area analysis, transit network understanding, and identifying route IDs for use in stop and prediction queries. AI agents should use this when users ask "list all CTA bus routes", "what routes serve downtown Chicago", or need to identify route IDs for subsequent CTA Bus Tracker queries.

List all CTA bus routes in Chicago
- **get_bus_stops**: Returns stop IDs (stpid), stop names, geographic coordinates (latitude, longitude), stop sequence order, and direction information (northbound, southbound, eastbound, westbound). Essential for stop discovery, journey planning, accessibility mapping, and identifying stop IDs for use in arrival prediction queries. AI agents should use this when users ask "list all stops on route 22 Clark", "find bus stops along Michigan Avenue", or need to identify stop IDs for use in get_bus_predictions queries.

List all bus stops for a specific CTA bus route
- **get_bus_vehicles**: Returns vehicle IDs (vid), route IDs, latitude/longitude coordinates, heading direction, speed, trip designators, block IDs, destination descriptions, and pattern names. Can query all buses system-wide or filter by specific route ID for targeted route-level tracking. Essential for real-time bus fleet monitoring, passenger arrival estimation, route-level service awareness, and transit operations management. AI agents should reference this when users ask "where are all the buses on route 22", "track bus positions system-wide", or need real-time vehicle position data for fleet visualization.

Get real-time positions of active CTA bus vehicles system-wide or filtered by route
- **get_route_directions**: Returns direction IDs (0 or 1), direction names (e.g., "Northbound", "Southbound", "Eastbound", "Westbound"), and associated route metadata. Essential for understanding route patterns, direction identification for stop queries, and trip planning with correct directional awareness. AI agents should use this when users ask "what directions does route 22 serve", "is there a northbound option for route 36", or need directional metadata to understand bus route geometry and plan trips in the correct direction.

Get direction information for a specific CTA bus route
- **get_route_status**: Returns route IDs, route names, status indicators (GOOD DELAYS, SLOWLY, SEVERE DELAYS, PLANNED WORK, SERVICE DISRUPTION, SUSPENDED), and status descriptions. Essential for quick system-wide health checks, commute planning, and understanding overall CTA reliability at a glance. AI agents should reference this when users ask "how is CTA running today", "what lines are delayed", or need a quick overview of system-wide service status before detailed trip planning.

Get current status of all CTA train lines and bus routes
- **get_service_alerts**: Returns alert descriptions, affected routes and stations, severity levels, cause types (maintenance, incident, weather, special events, construction), start and end timestamps, detour information, and alternative service recommendations. Can query all alerts system-wide or filter by specific route. Essential for service disruption awareness, alternative route planning, passenger communication, and understanding system reliability. AI agents should use this when users ask "are there any delays on the Red Line", "is CTA running normally today", or need to check service reliability before planning CTA journeys.

Get current service alerts and disruptions across the CTA system
- **get_stop_details**: Returns stop ID, stop name, geographic coordinates (latitude, longitude), and any associated route information. Essential for stop identification, accessibility planning, transit network analysis, and passenger information. AI agents should use this when users ask "tell me about stop 1234", "where is this bus stop located", or need detailed stop metadata to contextualize transit queries and trip planning.

Get detailed information about a specific CTA bus stop
- **get_system_time**: Returns the official server timestamp in standard format. Useful for synchronizing local clocks with the CTA system, verifying API connectivity, testing authentication, and timestamp alignment for real-time data correlation. AI agents should use this as a connectivity check before making more complex queries, or when users need to verify API responsiveness and authentication validity.

Get the current CTA Bus Tracker system timestamp
- **get_train_arrivals**: Returns predicted arrival times in minutes, train run numbers, destination stations, line colors (Red, Blue, Brown, Green, Orange, Purple, Pink, Yellow), operating status (on-time, delayed, scheduled, unscheduled, approaching, boarding, departing), and whether the train is approaching or at the station. Essential for real-time L tracking, passenger waiting time estimation, trip timing, and connection coordination. AI agents should use this when users ask "when is the next Red Line train at Clark/Lake", "show upcoming trains at this station", or need real-time arrival predictions for a specific CTA L station. MapIds are 5-digit station identifiers (e.g., 40360 for Clark/Lake, 40900 for Jackson). Station IDs can be found in the CTA GTFS static data feed.

Get real-time train arrival predictions for a specific L station
- **get_train_positions**: Returns train run numbers, line colors, next station IDs, service types (train, 5-car, 8-car), heading directions (North, South, East, West, Northeast, Northwest, Southeast, Southwest), scheduled vs. real-time status, and delay indicators. Can query all trains system-wide or filter by specific line (Red, Blue, Brown, Green, Orange, Purple, Pink, Yellow). Essential for real-time train tracking, network-wide service awareness, fleet monitoring, and understanding train distribution across the L system. AI agents should reference this when users ask "where are all the Red Line trains", "show train positions on the Blue Line", or need to visualize train locations for operational monitoring or passenger information.

Get real-time positions of all active CTA trains system-wide or filtered by line


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CTA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is the next Red Line train arriving at Clark/Lake?"

**🤖 AI Agent:**
> Fetching arrivals for Clark/Lake (mapId: 40360)... Next Red Line trains: Howard — 3 minutes, approaching; 95th/Dan Ryan — 6 minutes, on-time; Howard — 10 minutes, scheduled; 95th/Dan Ryan — 14 minutes, on-time. All Red Line trains currently running on schedule with no delays reported. Trains arrive approximately every 4-6 minutes during peak hours.

---

**👤 You:**
> "Show me all CTA bus stops on route 22 Clark."

**🤖 AI Agent:**
> Fetching stops for route 22 Clark... I found 89 stops along this major north-south corridor. Key stops include: Howard Street (North end), Morse, Loyola, Granville, Bryn Mawr, Berwyn, Lawrence, Montrose, Irving Park, Belmont, Fullerton, North/Clybourn, Chicago Ave, Grand, Washington, Jackson, Harrison, Roosevelt, Cermak-Chinatown, 35th-Bronzeville, 47th, 51st, 55th-Garfield, 63rd, and 95th Street (South end). Would you like arrival predictions for a specific stop?

---

**👤 You:**
> "How is CTA running today? Any delays on the L or bus routes?"

**🤖 AI Agent:**
> Checking CTA route status... System overview: Red Line — GOOD, Blue Line — GOOD, Brown Line — GOOD, Green Line — GOOD, Orange Line — GOOD, Purple Line — GOOD, Pink Line — GOOD, Yellow Line — GOOD. All L lines currently running on schedule with no major disruptions. For bus routes, most routes are operating normally. Would you like me to check specific alerts for a particular line or route, or get arrival predictions for your commute?


## Installation & Usage

To install and use the **CTA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cta](https://vinkius.com/mcp/cta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
