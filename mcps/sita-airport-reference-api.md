# SITA Airport Reference API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sita-airport-reference-api)
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


## ❓ FAQ

**Q: What format are airport codes in?**
The API uses standard 3-letter IATA airport codes (e.g., 'LHR' for London Heathrow, 'JFK' for New York JFK, 'GRU' for São Paulo Guarulhos).

**Q: Is this a read-only API?**
Yes, all 3 tools are strictly read-only queries. The integration retrieves reference data and cannot modify anything in the SITA database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sita-airport-reference-api](https://vinkius.com/mcp/sita-airport-reference-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SITA Airport Reference API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sita-airport-reference-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SITA Airport Reference API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sita-airport-reference-api": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
