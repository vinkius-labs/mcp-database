# AeroDataBox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aerodatabox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time flight status, airport flight information displays (FIDS), historical flight data, and airport delay statistics directly from your AI agent.

## Description
Connect **AeroDataBox** to your AI agent to fetch comprehensive global aviation data using natural language. This server integrates real-time flight tracking, airport schedules, and operational delay metrics.

### What you can do

- **Real-Time Flight Tracking** — Query the nearest flight status or look up flights by specific dates using flight numbers.
- **Airport Flight Information (FIDS)** — Retrieve departures and arrivals for any airport using absolute or relative time windows.
- **Flight History** — Search past, current, and scheduled flight movements by flight number, registration, callsign, or ICAO24 hex code.
- **Airport Delays** — Analyze current or historical airport delay statistics to understand operational performance.

### How it works

1. Subscribe to this server
2. Enter your AeroDataBox API Key
3. Start querying aviation data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel & Logistics Teams** — Monitor flight statuses and airport delays dynamically.
- **Aviation Enthusiasts & Developers** — Build smart assistants that track flights and analyze airport performance.
- **Data Analysts** — Gather historical flight data and airport delay statistics without manual exports.


## Available Tools
- **get_global_delays**: Get current global delays
- **get_alert_subscription**: Get details of a specific flight alert subscription
- **convert_alert_subscription**: Convert an old subscription to the credit-based system
- **create_flight_alert**: Create a flight alert webhook subscription
- **delete_alert_subscription**: Delete a flight alert webhook subscription
- **get_airline_fleet**: Get active aircraft operated by a given airline
- **get_airport_delays_historical**: Get historical airport delays for a specific date
- **get_airport_delays_period**: Get historical airport delays for a period
- **get_flight_history**: Get flight history and schedule
- **get_global_delays_historical**: Get historical global delays
- **get_nearest_flight**: Get real-time status of the nearest flight by flight number
- **list_alert_subscriptions**: List all flight alert webhook subscriptions
- **refill_alert_balance**: Refill flight alert credit balance
- **get_airport_delays**: Get current airport delays
- **get_airport_routes_stats**: Get statistical route frequencies for an airport
- **get_airport_runways**: Get detailed physical and operational runway data for an airport
- **get_airports_by_ip**: Find closest airports based on IP address
- **get_alert_balance**: Check flight alert credit balance
- **get_distance_time**: Calculate distance and estimated flight time between two airports
- **get_fids_absolute**: Get airport departures and arrivals (absolute time range)
- **get_fids_relative**: Get airport departures and arrivals (relative time range)
- **get_flight_by_date**: Get flight status on a specific date
- **get_flight_delays**: Get historical punctuality statistics for a specific flight number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AeroDataBox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the real-time status of flight AA100."

**🤖 AI Agent:**
> I will query the real-time status for flight AA100 using the `get_nearest_flight` tool. Let me fetch the current departure, arrival, and aircraft details for you.

---

**👤 You:**
> "Show me the departures and arrivals at EGLL for the next 6 hours."

**🤖 AI Agent:**
> I will retrieve the flight information display (FIDS) for London Heathrow (EGLL) using the `get_fids_relative` tool with a duration of 360 minutes. Here are the scheduled flights...

---

**👤 You:**
> "What are the current delays at JFK airport?"

**🤖 AI Agent:**
> I will check the current operational delays at John F. Kennedy International Airport (KJFK) using the `get_airport_delays` tool to provide you with statistical insights.


## ❓ FAQ

**Q: How can I check the real-time status of a flight using its flight number?**
You can use the `get_nearest_flight` tool by passing the flight number (e.g., 'DL47'). The agent will retrieve the real-time flight status, including departure/arrival times and aircraft details.

**Q: How do I list upcoming departures and arrivals for a specific airport?**
Use the `get_fids_relative` tool with the airport's ICAO code (e.g., 'KLGA') and optional offset/duration parameters. This returns a list of scheduled flights within that relative time window.

**Q: Can I retrieve historical delay statistics for an airport?**
Yes, you can use the `get_airport_delays_historical` tool by providing the airport's ICAO code and a specific date (YYYY-MM-DD) to analyze past operational performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aerodatabox](https://vinkius.com/mcp/aerodatabox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AeroDataBox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aerodatabox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AeroDataBox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aerodatabox": {
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
