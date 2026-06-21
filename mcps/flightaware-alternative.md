# FlightAware MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flightaware-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flightaware-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flightaware-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time flight tracking, airport activity, weather reports, and aircraft data via FlightAware's AeroAPI.

## Description
Connect your **FlightAware AeroAPI** account to any AI agent to access global aviation intelligence through natural conversation.

### What you can do

- **Flight Tracking** — Get real-time status and historical data for any flight using flight numbers or aircraft registration
- **Airport Operations** — Monitor arrivals, departures, and scheduled flights for any airport worldwide using ICAO/IATA codes
- **Weather Insights** — Retrieve current METAR observations and TAF forecasts to understand flight conditions
- **Route & Track Analysis** — Inspect planned flight routes and detailed position history (tracks) for active or past flights
- **Fleet & Operator Data** — Look up aircraft ownership details and airline operator information

### How it works

1. Subscribe to this server
2. Enter your FlightAware AeroAPI Key
3. Start querying aviation data from Claude, Cursor, or any MCP client

### Who is this for?

- **Logistics & Operations** — Track cargo flights and monitor airport congestion in real-time
- **Aviation Enthusiasts** — Get deep technical data on specific aircraft and flight paths
- **Travelers & Concierges** — Stay updated on flight schedules and airport weather conditions


## Available Tools
- **get_aircraft**: Get information about a specific aircraft
- **get_operator_flights**: Get current and scheduled flights for an operator
- **get_operator**: Get details about a specific operator (airline)
- **get_airport_flights**: Get flights for a specific airport
- **get_airport_weather**: Get current weather and forecasts for an airport
- **get_flight_route**: Get the planned route for a specific flight
- **get_flight_track**: Get the track (position history) for a specific flight
- **get_flights**: g., flight number or registration).

Get flights for a specific identifier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FlightAware** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track flight SWA1234 and show me its current status."

**🤖 AI Agent:**
> I've retrieved the data for SWA1234. It is currently airborne, flying from Dallas (DAL) to Austin (AUS). Current altitude is 24,000 ft with an estimated arrival in 15 minutes.

---

**👤 You:**
> "What is the weather and forecast for London Heathrow (EGLL)?"

**🤖 AI Agent:**
> The current METAR for EGLL shows winds from 270 at 10kts, visibility 10km+, and scattered clouds at 3,000ft. The TAF forecast indicates clear conditions continuing for the next 6 hours.

---

**👤 You:**
> "Show me the planned route for flight DLH400."

**🤖 AI Agent:**
> The planned route for DLH400 (Frankfurt to New York) includes waypoints: OBOKA L607 SPI UT420 TNT. It is scheduled to fly at a cruise altitude of FL340.


## Installation & Usage

To install and use the **FlightAware** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flightaware-alternative](https://vinkius.com/mcp/flightaware-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
