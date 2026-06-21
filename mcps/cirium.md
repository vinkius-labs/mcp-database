# Cirium MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cirium)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cirium-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cirium-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Automate flight tracking and aviation data via Cirium — monitor flight statuses, airport traffic, and global schedules directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cirium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the status of flight AA 100 for October 25th, 2023?"

**🤖 AI Agent:**
> I'm checking the status for American Airlines flight 100 on 2023-10-25. The flight departed JFK on time at 18:15 and is currently estimated to arrive at LHR at 06:20 local time.

---

**👤 You:**
> "Show me all flights scheduled between LAX and JFK for tomorrow."

**🤖 AI Agent:**
> I've retrieved the schedules for the LAX to JFK route. There are 12 scheduled flights tomorrow, including Delta DL442 at 08:00 and JetBlue B624 at 10:30. Would you like details on a specific one?

---

**👤 You:**
> "Where is flight DL 456 right now?"

**🤖 AI Agent:**
> Fetching the current track for Delta flight 456... The aircraft is currently over the Atlantic at 35,000 feet, heading Northeast at 540 knots. It is approximately 2 hours from its destination.


## Installation & Usage

To install and use the **Cirium** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cirium](https://vinkius.com/mcp/cirium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
