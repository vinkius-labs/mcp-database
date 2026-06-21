# OpenSky Network MCP Server

Track real-time flights, view aircraft states, and get airport arrivals/departures via OpenSky API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opensky-network)

## Overview
**Category:** the-unthinkable
**Tools Count:** 8

## Description
Connect **OpenSky Network** to any AI agent and access global, open-source air traffic data -- track aircraft in real-time, view historical flights, and monitor airport activity through natural conversation.

### What you can do
- **Real-Time Tracking** -- Get the current state of all tracked aircraft including altitude, velocity, and location
- **Airport Monitoring** -- View recent arrivals and departures for any ICAO airport code
- **Aircraft History** -- Retrieve recent flight history and tracks for specific aircraft by ICAO24 hex code
- **Flight Intervals** -- Get all flights that occurred within a specific time window
- **Account Tracking** -- Monitor your own registered aircraft (requires authentication)

### How it works
1. Subscribe to this server
2. (Optional) Enter your OpenSky credentials for higher rate limits
3. Start tracking global aviation data from Claude, Cursor, or any MCP-compatible client

OpenSky Network is the largest open-source air traffic data platform, providing free access to ADS-B and other aviation telemetry.

### Who is this for?
- **Aviation Enthusiasts** -- Track specific aircraft and monitor local airport traffic
- **Logistics Teams** -- Monitor estimated arrival times and flight statuses
- **Data Analysts** -- Access historical flight data for trend analysis and research


## Available Tools
- **get_all_states**: Optionally filter by specific ICAO24 code.

Get the states of all aircraft currently tracked by OpenSky
- **get_arrivals**: Get arrivals at a specific airport
- **get_departures**: Get departures from a specific airport
- **get_flights_by_aircraft**: Get historical flights for a specific aircraft
- **get_flights_by_interval**: Requires authentication.

Get all flights in a specific time interval
- **get_my_flights**: Get historical flights for your own aircraft (requires authentication)
- **get_my_states**: Get the states of your own aircraft (requires authentication)
- **get_recent_tracks**: Get recent tracks for a specific aircraft


## Installation & Usage

To install and use the **OpenSky Network** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensky-network](https://vinkius.com/mcp/opensky-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
