# AeroAPI (FlightAware) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aeroapi-flightaware)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aeroapi-flightaware-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aeroapi-flightaware-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track global flights — audit departures, arrivals, and airports via IA.

## Description
Empower your AI agent to orchestrate your entire aviation research and flight auditing workflow with **AeroAPI**, the authoritative source for real-time flight data from FlightAware. By connecting AeroAPI to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly track flights by identifier, audit airport arrival and departure schedules, and retrieve detailed airport metadata without you ever touching a flight tracker. Whether you are conducting supply chain research or monitoring travel logistics, your agent acts as a real-time aviation consultant, ensuring your data is always precise and up-to-the-minute.

### What you can do

- **Flight Auditing** — Retrieve high-resolution details for any specific flight, including status, origin, and destination metadata.
- **Airport Oversight** — Audit arrival and departure schedules for global airports to maintain a clear view of maritime logistics and distribution.
- **Geographic Discovery** — Search for flights based on regional queries to understanding the current industry lead in aviation flow instantly.
- **Metadata Intelligence** — Retrieve unique airport codes and timezone information to assist in deep-dive logistics classification.
- **Operational Monitoring** — Check API status to ensure your aviation research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your FlightAware AeroAPI Key
3. Start managing your aviation intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Logistics Managers** — monitor flight timelines and retrieve arrival metadata straight from your workflow.
- **Aviation Researchers** — verify airport schedules and audit global flight patterns without manual searching.
- **Travel Operations** — perform rapid audits of flight statuses and identify relevant airport markers through natural language.
- **Operations Leads** — automate aviation data querying to orchestrate cross-functional logistics teams smoothly.


## Available Tools
- **check_api_status**: Check if the AeroAPI service is operational
- **get_airport_details**: Get metadata and location details for a specific airport by code (ICAO or IATA)
- **get_flight_details**: Get comprehensive details for a specific flight by identifier (ident or fa_flight_id)
- **list_airport_flights**: List scheduled, enroute, or arrived flights for a specific airport
- **search_flights**: Search for flights based on a query (e.g., origin, destination, ident)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AeroAPI (FlightAware)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for flight 'DAL123' using AeroAPI."

**🤖 AI Agent:**
> I've retrieved the details for flight DAL123! It is currently identified as 'En Route' from Atlanta (ATL) to New York (JFK). The estimated arrival time is 2:30 PM. Would you like the full enroute metadata for this flight?

---

**👤 You:**
> "List arrivals for airport 'LHR' (London Heathrow)."

**🤖 AI Agent:**
> I've retrieved the arrival schedule for London Heathrow! Notable incoming flights include BA214 from New York and AF1680 from Paris. I can provide the status and gate metadata for each of these arrivals if you'd like.

---

**👤 You:**
> "What are the metadata details for airport 'KJFK'?"

**🤖 AI Agent:**
> I've retrieved the metadata for John F. Kennedy International Airport (KJFK). It is located in New York, USA, and uses the America/New_York timezone. I can assist you with more geographic and operational markers for this site if you'd like.


## Installation & Usage

To install and use the **AeroAPI (FlightAware)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aeroapi-flightaware](https://vinkius.com/mcp/aeroapi-flightaware)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
