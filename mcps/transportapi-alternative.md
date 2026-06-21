# TransportAPI MCP Server

UK public transport intelligence — live departures, journey planning, train fares, timetables, and postcode-based station search via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/transportapi-alternative)

## Overview
**Category:** data-analytics
**Tools Count:** 12

## Description
Empower your AI agent to orchestrate your entire public transport research workflow with **TransportAPI**, Britain's leading platform for transport data. By connecting TransportAPI to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly search for stations, audit live bus and train departures, and retrieve detailed journey plans without you ever touching a travel app. Whether you are conducting urban mobility research or monitoring daily commute patterns, your agent acts as a real-time transit consultant, ensuring your data is always comprehensive and up-to-date.

### What you can do

- **Departure Auditing** — Query real-time bus and train departures for any stop or station to maintain a clear view of local transit flow.
- **Journey Oversight** — Plan public transport routes between any locations and retrieve detailed itinerary metadata, including aimed vs expected times.
- **Station Discovery** — Search for train stations and bus stops by keyword or retrieve nearby transport hubs based on geographic coordinates.
- **Service Intelligence** — Query specific bus and train service details, including operator information and full route timetables.
- **Logistics Monitoring** — List available routes and service statuses to maintain strict control over urban transport data.

### How it works

1. Subscribe to this server
2. Enter your TransportAPI App ID and API Key
3. Start managing your transport intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Urban Researchers** — monitor public transport patterns and retrieve live transit metadata straight from your workflow.
- **Logistics Managers** — verify service reliability and audit operator performance across different lines.
- **Daily Commuters** — perform rapid audits of nearby departures and identify the best routes through natural language.
- **Operations Leads** — automate transport data querying to orchestrate cross-functional mobility teams smoothly.


## Available Tools
- **get_bus_service**: Get details of a bus service route
- **get_bus_route_timetable**: Get the scheduled timetable for a bus route
- **get_transport_by_postcode**: Useful when user only has a postcode, not coordinates.

Find transport options by UK postcode
- **get_live_bus_departures**: Returns live departure times, destinations, and operators.

Get real-time bus departures for a UK bus stop
- **get_live_train_departures**: g., KGX for King's Cross, PAD for Paddington).

Get real-time train departures for a UK station
- **get_nearby_bus_stops**: Find bus stops near a GPS location
- **get_nearby_transport_places**: Find transport locations near GPS coordinates
- **get_train_fares**: Great for price comparison.

Get ticket prices between two stations
- **get_train_service_details**: Get the full calling pattern of a train service
- **get_train_station_timetable**: Get the scheduled timetable for a train station
- **plan_public_transport_journey**: Returns step-by-step route with times and changes.

Plan a public transport journey between two locations
- **search_transport_places**: Search for train stations and bus stops by name


## Installation & Usage

To install and use the **TransportAPI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transportapi-alternative](https://vinkius.com/mcp/transportapi-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
