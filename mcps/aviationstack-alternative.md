# AviationStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aviationstack-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Real-time flight tracking and global aviation data — monitor flights, routes, airports, and airline schedules directly from any AI agent.

## Description
Connect **AviationStack** to your AI agent to unlock a world of aviation intelligence. Whether you are tracking a specific flight, analyzing global routes, or managing travel logistics, this server provides the real-time data you need.

### What you can do

- **Flight Tracking** — Get real-time status updates for active flights or look up historical data using flight numbers and dates via `list_flights`.
- **Global Infrastructure** — Access comprehensive lists of airports, cities, and countries with IATA/ICAO codes and timezones using `list_airports` and `list_cities`.
- **Airline Intelligence** — Query airline details, aircraft types, and specific airplane registrations with `list_airlines` and `list_airplanes`.
- **Route Planning** — Inspect scheduled airline routes and timetables to understand global connectivity using `list_routes` and `list_timetable`.
- **Future Schedules** — Access upcoming flight schedules with `list_future_flights` (requires Professional plan or higher).

### How it works

1. Subscribe to this server
2. Enter your AviationStack API Access Key
3. Start querying aviation data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel & Logistics Teams** — Monitor flight statuses and coordinate arrivals/departures seamlessly.
- **Developers** — Integrate aviation data into applications without building complex scrapers.
- **Data Analysts** — Analyze historical flight patterns and global route connectivity.


## Available Tools (11)
- **list_aircraft_types**: Get aircraft types and specifications
- **list_cities**: Get cities worldwide
- **list_airlines**: Get global airlines list
- **list_timetable**: Requires Professional plan or higher.

Get airport timetables
- **list_airplanes**: Get specific aircraft details
- **list_airports**: Get global airports list
- **list_countries**: Get countries worldwide
- **list_flights**: Use flight_date for historical data.

Get real-time and historical flight data
- **list_future_flights**: Requires Professional plan or higher.

Get future flight schedules
- **list_routes**: Get scheduled airline routes
- **list_taxes**: Get aviation taxes information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AviationStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of flight LH400?"

**🤖 AI Agent:**
> I'm checking the real-time data for LH400... The flight is currently 'active', departed from Frankfurt (FRA) at 10:45 AM and is estimated to land in New York (JFK) at 1:20 PM local time.

---

**👤 You:**
> "List all airports in Tokyo."

**🤖 AI Agent:**
> Fetching airports for Tokyo... I found Narita International (NRT) and Haneda Airport (HND). Would you like the specific ICAO codes or timezone details for these?

---

**👤 You:**
> "Show me the scheduled routes for Emirates."

**🤖 AI Agent:**
> Querying airline routes... I've retrieved the latest scheduled routes for Emirates. They include major hubs like Dubai (DXB) to London (LHR), Paris (CDG), and Singapore (SIN). Shall I list more specific route details?


## ❓ FAQ

**Q: Can I track a specific flight using its flight number?**
Yes. Use the `list_flights` tool and provide the `flight_number`. You can also filter by `airline_name` or status like 'active' or 'landed'.

**Q: How do I find the IATA code for a specific airport?**
You can use the `list_airports` tool to retrieve a global list of airports, which includes their IATA and ICAO codes, locations, and timezones.

**Q: Does this server support historical flight data?**
Yes. By using the `list_flights` tool with the `flight_date` parameter (YYYY-MM-DD), you can access historical flight records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aviationstack-alternative](https://vinkius.com/mcp/aviationstack-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AviationStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aviationstack-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AviationStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aviationstack-alternative": {
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
