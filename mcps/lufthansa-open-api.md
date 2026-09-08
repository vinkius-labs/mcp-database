# Lufthansa Open API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lufthansa-open-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

The official Lufthansa Open API as an MCP: airport/country/airline reference data, nearest-airports, flight schedules, live flight status by flight or route, and lounge finders — OAuth client_credentials auth.

## Description
The **official Lufthansa Open API** (Lufthansa Developer Network) as a single MCP server — operational and reference data for the Lufthansa Group (Lufthansa, SWISS, Austrian, Brussels Airlines, Discover).

### What you can do
- **Reference data** — airports (FRA, MUC, LIS...), countries and airlines by code, with multilingual names, coordinates and time zones
- **Nearest airports** — official LH list of airports sorted by distance from any coordinate
- **Flight schedules** — the LH Group timetable between two airports for a date window: flight numbers, times, aircraft, days of operation
- **Live flight status** — one flight (LH1178 on 2026-09-07) or a whole route between date-times: scheduled/estimated/actual times, gates, delays
- **Lounges** — LH Group lounges at an airport filtered by cabin class (First/Business/Economy)

### Authentication (from the official Getting Started docs)
1. Register at **developer.lufthansa.com** to get a Client ID + Client Secret
2. The MCP mints a token at `POST https://api.lufthansa.com/v1/oauth/token` (`grant_type=client_credentials`, form-encoded) — bearer tokens expire after a limited time and are auto-refreshed here
3. Every call goes to `https://api.lufthansa.com/v1/...` with `Accept: application/json` (XML available in the API if preferred)

### Who is this for?
Travel apps, flight-watch and timetable agents, airport/lounge assistants, aviation analysts and anyone building on authoritative Lufthansa Group data.


## Available Tools (8)
- **get_airport**: Use IATA codes like FRA, MUC, LIS.

Get Lufthansa master data for an airport by IATA code (name, coordinates, timezone)
- **get_country**: Use 2-letter ISO codes (DE, PT, US).

Get Lufthansa country reference by ISO code
- **get_airline**: LH=Lufthansa, SN=Brussels Airlines, OS=Austrian, EN=Discover.

Get Lufthansa airline reference by IATA code (LH, SN, OS, EN...)
- **get_nearest_airports**: Great for "which airports are near this city?" and travel planning.

Find airports nearest to a coordinate pair (with distance in km)
- **get_flight_schedules**: fromDateTime ISO (YYYY-MM-DDTHH:mm) with optional days & limit paging; also paginate via offset.

Get scheduled LH Group flights between two airports for a period (timetable)
- **get_flight_status**: Flight number like "LH1178"; date YYYY-MM-DD. Requires the Flight Status product on your LH key.

Get live flight status for one LH Group flight number on a date (delays, gates, actual times)
- **get_flight_status_range**: from/to ISO (YYYY-MM-DDTHH:mm). Requires the Flight Status product.

Get flight status for a route between two date-times (status board per route)
- **get_lounges**: Returns lounge names, locations, opening hours within the airport. Requires the Lounges product on your LH key.

Find LH Group lounges at an airport filtered by cabin class (hype: lounge access checks)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lufthansa Open API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is LH1178 on time today?"

**🤖 AI Agent:**
> 🛩️ **LH1178 — 2026-09-07 (Lufthansa Open API)**

Route: Frankfurt (FRA) → Lisbon (LIS)
Status: Departed
Scheduled: 10:30 CEST → Estimated: 10:30 CEST (on time)
Gate/terminal and actual times in the payload.

Want the return leg or tomorrow's schedule?

---

**👤 You:**
> "Which airports are near downtown Lisbon?"

**🤖 AI Agent:**
> 📍 **Nearest airports to 38.72, -9.14 (LH reference)**

1. LIS — Lisbon Humberto Delgado, ~6 km
2. Other LH-served airports sorted by distance...

Official distance list straight from the mds-references API. Want schedules from the top result?

---

**👤 You:**
> "Show me Business class lounges at Munich airport"

**🤖 AI Agent:**
> 🛋️ **LH Group lounges @ MUC (Business)**

- Lufthansa Business Lounge, Terminal 2, Level 4 (near G24)
- Satellite Terminal Business Lounge
- Opening hours and access rules in the payload.

Flying First? I can re-query with cabin F for the First Class Terminal.


## ❓ FAQ

**Q: How do I get the Client ID/Secret?**
Register a free account at developer.lufthansa.com and create an app — the portal issues a client key (ID) and secret. The MCP exchanges them at POST /v1/oauth/token (grant_type=client_credentials) for a bearer token and refreshes it automatically when it expires.

**Q: Which products does my key cover?**
Reference data (airports/countries/airlines/nearest-airports) and flight schedules are typically available on the free tier. Flight Status, Lounges and Seat Maps are separate products you must enable when registering the app — a key without them returns the gateway's 'Account Inactive'/permission error on those paths.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lufthansa-open-api](https://vinkius.com/ai-agent-connect/lufthansa-open-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lufthansa Open API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lufthansa-open-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lufthansa Open API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lufthansa-open-api": {
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
