# Boeing Developer Tools MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boeing-developer-tools)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/boeing-developer-tools-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/boeing-developer-tools-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Global aviation intelligence, Jeppesen aerodromes, and aircraft models.

## Description
Connect your natural language AI directly to the **Boeing Developer Tools (BDT)** ecosystem. Take full control of aviation data, flight intelligence, and global airport restrictions without intermediary data scrapers.

### What you can do

- **Flight Intelligence** — Query real-time tracking, constraints, and live statuses for individual commercial flights
- **Jeppesen Aerodromes** — Scan physical metadata, coordinates, and ground operations for nearly every airport via ICAO
- **Runways & Taxi Times** — Consult active taxiing delays and runway monitor metrics in highly congested airports
- **Urgent NOTAMs** — Read critical Notice to Air Missions immediately to understand airspace constraints or closures
- **Aircraft Specifications** — Validate dimensions, configurations, and specs parameters for Boeing models
- **Parts Inventory** — Check availability, lifecycle, and pricing catalogs for specific Boeing components

### How it works

1. Subscribe to this server
2. Enter your Boeing Aviation ID Bearer token
3. Start fetching high-fidelity aviation reports straight from Claude, Cursor, or any MCP-compatible agent

### Who is this for?

- **Aviation Analysts** — map exact airport constraints and live NOTAM restrictions without crawling raw PDFs
- **Operations Teams** — instantly diagnose fleet ground delays, fetching real-time Jeppesen taxi times automatically
- **Aircraft Engineers** — find precise parts inventory and structural metrics without leaving the development workflow


## Available Tools
- **get_runway_monitor**: Real-time airport runway congestion monitor
- **check_part_availability**: Check Boeing part stock availability & pricing
- **get_aerodrome_details**: Get thorough Jeppesen data for an airport/aerodrome
- **get_aircraft_specs**: Get detailed Boeing aircraft model specifications
- **get_airspace_info**: Retrieve airspace restrictions and metadata
- **get_flight_events**: Get real-time flight tracking events and status
- **get_taxi_time**: Get real-time taxi times for an airport
- **search_notams**: Search for Notice to Air Missions (NOTAMs)
- **search_boeing_parts**: Search the Boeing global aviation supply chain
- **search_runways**: Search for runways and parameters of an airport


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Boeing Developer Tools** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pull the physical specifications, wing dimensions and fuel range for the Boeing 787 model family using the aircraft tools."

**🤖 AI Agent:**
> Extracting aircraft metadata for '787'... According to the Boeing catalog, the 787-9 Dreamliner has a primary wingspan of 60.12 meters (197 ft 3 in) and its Maximum Fuel Capacity reaches up to 126,206 Liters, equating to roughly a 14,140 KM range under optimal weight parameters. Do you want specifics on engine thrust output?

---

**👤 You:**
> "Check the current runway monitor and taxi time delays for airport ICAO code EDDF (Frankfurt)."

**🤖 AI Agent:**
> Querying Jeppesen runway feeds for EDDF... Ground monitoring reports a steady Operational flow. Real-time outbound taxi times average 14.5 minutes. Operations and runway lighting loops are entirely stable. No major congestion events identified at Frankfurt right now.

---

**👤 You:**
> "Search the most critical active NOTAMs at KJFK (JFK Airport) right now and summarize any airspace closures."

**🤖 AI Agent:**
> Pulling the NOTAM list for the KJFK scope. I identified 4 active notices. The only critical closure states: **TWY A BTN TWY A1 AND TWY A2 CLSD** (meaning Taxiway A is strictly closed between Alpha 1 and Alpha 2 for surface restructuring until tonight). There are no broader airspace or active runway closures in effect.


## Installation & Usage

To install and use the **Boeing Developer Tools** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boeing-developer-tools](https://vinkius.com/mcp/boeing-developer-tools)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
