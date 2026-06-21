# FlightStats MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flightstats)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flightstats-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flightstats-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track real-time flight statuses, routes, airport departures/arrivals, and flight paths directly from your AI agent.

## Description
Connect **FlightStats** to your AI agent to monitor global aviation data, track active flights, and query airport schedules using natural language.

### What you can do

- **Real-Time Flight Status** — Query live flight progress, delays, and gate information using `get_flight_status`.
- **Positional Tracking** — Retrieve coordinates, speed, and altitude for active flights with `get_flight_track`.
- **Airport Boards** — List departures and arrivals for any global airport during specific hours using `get_airport_status`.
- **Route Monitoring** — Analyze all flights operating between two airports on a given day via `get_route_status`.
- **Geospatial Queries** — Find active flights flying within a specific radius of any coordinate using `get_flights_near`.

### How it works

1. Subscribe to this server
2. Enter your FlightStats App ID and App Key
3. Start tracking flights and airport schedules directly from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_active_airlines**: Get all active airlines
- **get_active_airports**: Get all active airports
- **get_airport_by_code**: Get airport details by code
- **get_airport_status**: Get flight status for departures or arrivals at an airport
- **get_connections**: Get connecting flight options between two airports
- **create_multi_flight_alert**: Create an alert rule for all flights arriving at an airport
- **create_single_flight_alert**: Requires a configured callback URL on the account.

Create an alert rule for a single flight
- **get_delay_index**: 0 to 5.0) based on recent departure delays and cancellations.

Get delay index for an airport
- **get_equipment_by_code**: Get aircraft equipment details by IATA code
- **get_fids**: Get Flight Information Display System (FIDS) data
- **get_flight_status**: Available from ~3 days before departure to 7 days after arrival.

Get real-time flight status by carrier and flight number
- **get_flight_track**: Get real-time flight track and positional information
- **get_flights_near**: Get flights near a geographic area
- **get_historical_airport_status**: Get historical flight status for airport departures
- **get_historical_flight_status**: Get historical flight status by flight
- **get_historical_route_status**: Get historical flight status for a route
- **get_ratings_by_flight**: Get on-time performance ratings for a flight
- **get_ratings_by_route**: Get on-time performance ratings for a route
- **get_route_status**: Get flight status for a specific route
- **get_scheduled_flights_by_flight**: Get future scheduled flights by carrier and flight number
- **get_scheduled_flights_by_route**: Get future scheduled flights by route
- **get_weather**: Get weather (METAR/TAF) for an airport


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FlightStats** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status of flight UA 240 departing today."

**🤖 AI Agent:**
> I've queried `get_flight_status` for United Airlines flight 240. The flight is currently on schedule, departing from Gate C12 at 3:45 PM and estimated to arrive at 6:12 PM.

---

**👤 You:**
> "What are the arrivals at Heathrow (LHR) airport for the 14:00 hour today?"

**🤖 AI Agent:**
> Using `get_airport_status` for LHR arrivals at 14:00, I found 12 scheduled flights. Notable arrivals include BA 212 from Boston (landed early at 13:50) and VS 104 from Atlanta (delayed to 14:15).

---

**👤 You:**
> "Find active flights within 25 miles of coordinates 45.515, -122.679."

**🤖 AI Agent:**
> Invoking `get_flights_near`... I detected 3 active flights in this radius: AS 342 (Boeing 737 at 12,000ft), QX 5021 (Embraer E175 descending to PDX), and UA 1822 (Airbus A320 cruising at 34,000ft).


## Installation & Usage

To install and use the **FlightStats** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flightstats](https://vinkius.com/mcp/flightstats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
