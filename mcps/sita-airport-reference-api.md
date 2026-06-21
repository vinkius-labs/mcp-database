# SITA Airport Reference API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sita-airport-reference-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sita-airport-reference-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sita-airport-reference-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Query global airport infrastructure data — IATA codes, terminals, gates, and reference metadata via AI.

## Description
Access the **SITA Airport Reference API** through natural conversation with your AI agent. This integration provides programmatic access to the world's most comprehensive airport reference database, maintained by SITA — the global leader in air transport IT solutions.

### What you can do

- **Airport Directory** — List all global airports registered in the SITA database with their IATA codes, names, and locations
- **Airport Details** — Retrieve comprehensive metadata for any airport including timezone, coordinates, city, country, and operational data
- **Terminal Intelligence** — List all terminals, concourses, and gate areas for a specific airport

### How it works

1. Subscribe to this server
2. Register at the [**SITA Developer Portal**](https://www.developer.aero/) and obtain your API Key
3. Start querying airport infrastructure data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Aviation Developers** — integrate airport metadata into flight tracking and booking applications
- **Travel Tech Companies** — enrich travel products with accurate terminal and gate information
- **Airport Operations** — programmatic access to reference data for planning and analytics


## Available Tools
- **get_airport_reference_details**: Use the 3-letter IATA code (e.g., "LHR", "JFK", "GRU").

Get full reference metadata for a specific airport by code (IATA)
- **list_sita_airports**: List all global airports registered in the SITA database
- **list_airport_terminals**: Useful for flight operations, passenger routing, and airport infrastructure planning.

List all terminals and gate areas for a specific airport


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SITA Airport Reference API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all the terminals at London Heathrow Airport."

**🤖 AI Agent:**
> I've retrieved the terminal information for LHR. London Heathrow has 4 active terminals: Terminal 2 (The Queen's Terminal), Terminal 3, Terminal 4, and Terminal 5. Would you like details on a specific terminal?

---

**👤 You:**
> "Get the full details for São Paulo Guarulhos airport."

**🤖 AI Agent:**
> Here are the details for GRU (São Paulo/Guarulhos International Airport): Location: Guarulhos, São Paulo, Brazil. Timezone: America/Sao_Paulo (UTC-3). IATA: GRU, ICAO: SBGR. Coordinates: -23.4356, -46.4731. Would you like to see the terminal layout?


## Installation & Usage

To install and use the **SITA Airport Reference API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sita-airport-reference-api](https://vinkius.com/mcp/sita-airport-reference-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
