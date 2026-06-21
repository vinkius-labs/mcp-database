# OpenSky Network MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opensky-network)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opensky-network-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opensky-network-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Track real-time flights, view aircraft states, and get airport arrivals/departures via OpenSky API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSky Network** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all current flights near my location."

**🤖 AI Agent:**
> Found 3 aircraft nearby: 1. Delta 456 (A320) at 10,000ft. 2. Private Cessna (C172) at 3,500ft.

---

**👤 You:**
> "Track the aircraft with ICAO24 code a1b2c3."

**🤖 AI Agent:**
> Aircraft a1b2c3: Altitude 35,000ft, Velocity 450 kts, Location 40.7128, -74.0060.

---

**👤 You:**
> "What flights departed from EDDF in the last 2 hours?"

**🤖 AI Agent:**
> Found 45 departures from EDDF: 1. Lufthansa 400 to KJFK. 2. United 960 to ORD.


## Installation & Usage

To install and use the **OpenSky Network** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensky-network](https://vinkius.com/mcp/opensky-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
