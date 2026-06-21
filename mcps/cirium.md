# Cirium MCP Server

Automate flight tracking and aviation data via Cirium — monitor flight statuses, airport traffic, and global schedules directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cirium)

## Overview
**Category:** data-analytics
**Tools Count:** 9

## Description
Connect your **Cirium** developer account to any AI agent to access the world's most comprehensive aviation data through natural conversation.

### What you can do

- **Flight Status & Tracking** — Get real-time updates on commercial flights and track their current GPS positions and flight paths using `get_flight_status` and `get_flight_track`.
- **Airport Operations** — Monitor departures and arrivals for any major airport by IATA code with `get_airport_status`, including specific hourly windows.
- **Route Analysis** — Query all active flights between two cities using `get_route_status` to understand delays or availability on specific routes.
- **Fleet Monitoring** — Inspect the status of an entire airline's fleet with `get_fleet_status` to see active airborne assets.
- **Global Schedules** — Access planned flight schedules and connection data for future planning via `get_schedules_by_route` and `get_schedules_by_carrier`.

### How it works

1. Subscribe to this server
2. Enter your Cirium App ID and App Key
3. Start querying aviation data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics & Travel Managers** — instantly check flight delays and reschedule connections without manual searching.
- **Aviation Professionals** — monitor fleet movements and airport congestion directly from your workflow.
- **Developers & Data Analysts** — pull real-time positional data and schedules into your AI-driven tools.


## Available Tools
- **get_airport_status**: Get a list of flights departing from or arriving at an airport
- **get_airport_tracks**: Get tracks for all flights near a specific airport
- **create_alert_rule**: Register a new alert rule for a flight
- **get_fleet_status**: Get status for all flights in a carrier fleet
- **get_flight_status**: Get status for a specific flight on a specific date
- **get_schedules_by_route**: Get scheduled flights between two airports for a date
- **get_flight_track**: Get the current position and track for a specific flight
- **get_route_status**: Get status for all flights between two airports
- **get_schedules_by_carrier**: Get scheduled flights for a specific carrier on a date


## Installation & Usage

To install and use the **Cirium** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cirium](https://vinkius.com/mcp/cirium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
