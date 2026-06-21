# AeroDataBox MCP Server

Access real-time flight status, airport flight information displays (FIDS), historical flight data, and airport delay statistics directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/aerodatabox)

## Overview
**Category:** data-analytics
**Tools Count:** 23

## Description
Connect **AeroDataBox** to your AI agent to fetch comprehensive global aviation data using natural language. This server integrates real-time flight tracking, airport schedules, and operational delay metrics.

### What you can do

- **Real-Time Flight Tracking** — Query the nearest flight status or look up flights by specific dates using flight numbers.
- **Airport Flight Information (FIDS)** — Retrieve departures and arrivals for any airport using absolute or relative time windows.
- **Flight History** — Search past, current, and scheduled flight movements by flight number, registration, callsign, or ICAO24 hex code.
- **Airport Delays** — Analyze current or historical airport delay statistics to understand operational performance.

### How it works

1. Subscribe to this server
2. Enter your AeroDataBox API Key
3. Start querying aviation data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel & Logistics Teams** — Monitor flight statuses and airport delays dynamically.
- **Aviation Enthusiasts & Developers** — Build smart assistants that track flights and analyze airport performance.
- **Data Analysts** — Gather historical flight data and airport delay statistics without manual exports.


## Available Tools
- **get_global_delays**: Get current global delays
- **get_alert_subscription**: Get details of a specific flight alert subscription
- **convert_alert_subscription**: Convert an old subscription to the credit-based system
- **create_flight_alert**: Create a flight alert webhook subscription
- **delete_alert_subscription**: Delete a flight alert webhook subscription
- **get_airline_fleet**: Get active aircraft operated by a given airline
- **get_airport_delays_historical**: Get historical airport delays for a specific date
- **get_airport_delays_period**: Get historical airport delays for a period
- **get_flight_history**: Get flight history and schedule
- **get_global_delays_historical**: Get historical global delays
- **get_nearest_flight**: Get real-time status of the nearest flight by flight number
- **list_alert_subscriptions**: List all flight alert webhook subscriptions
- **refill_alert_balance**: Refill flight alert credit balance
- **get_airport_delays**: Get current airport delays
- **get_airport_routes_stats**: Get statistical route frequencies for an airport
- **get_airport_runways**: Get detailed physical and operational runway data for an airport
- **get_airports_by_ip**: Find closest airports based on IP address
- **get_alert_balance**: Check flight alert credit balance
- **get_distance_time**: Calculate distance and estimated flight time between two airports
- **get_fids_absolute**: Get airport departures and arrivals (absolute time range)
- **get_fids_relative**: Get airport departures and arrivals (relative time range)
- **get_flight_by_date**: Get flight status on a specific date
- **get_flight_delays**: Get historical punctuality statistics for a specific flight number


## Installation & Usage

To install and use the **AeroDataBox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aerodatabox](https://vinkius.com/mcp/aerodatabox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
