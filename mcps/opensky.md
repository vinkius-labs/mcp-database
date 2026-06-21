# OpenSky MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opensky)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time and historical global flight tracking data — monitor aircraft states, flight trajectories, and airport traffic directly from your AI agent.

## Description
Connect to the **OpenSky Network** to integrate comprehensive aviation intelligence into your AI workflows. This server provides access to a massive crowdsourced dataset of flight tracking data, allowing for deep analysis of global air traffic.

### What you can do

- **Real-time Tracking** — Fetch live state vectors (position, velocity, altitude) for aircraft globally or within specific geographic boundaries.
- **Historical Flight Data** — Retrieve detailed flight logs for specific aircraft (ICAO24) or entire time intervals to analyze past movements.
- **Airport Operations** — Monitor arrivals and departures for any airport using ICAO codes to understand traffic flow and scheduling.
- **Trajectory Analysis** — Extract the precise track and path of a specific flight to visualize or analyze its route.
- **Global Overview** — Query all historical flights occurring within a specific window for large-scale data analysis.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OpenSky Network credentials for higher rate limits
3. Start querying live aviation data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — Perform large-scale aviation research and trend analysis using historical flight data.
- **Logistics & Supply Chain** — Monitor cargo flight movements and airport congestion in real-time.
- **Aviation Enthusiasts** — Track specific aircraft or monitor local airspace through natural language commands.


## Available Tools
- **get_flights_by_aircraft**: Retrieve historical flights for a specific aircraft
- **get_flights_all**: Retrieve all historical flights in a time interval
- **get_flights_by_arrival**: Retrieve historical flights arriving at an airport
- **get_flights_by_departure**: Retrieve historical flights departing from an airport
- **get_states**: Can be filtered by time, specific aircraft (icao24), or a geographic bounding box.

Retrieve real-time aircraft state vectors
- **get_tracks**: Retrieve the trajectory of a specific flight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenSky** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the current state vectors for aircraft with ICAO24 'a80c3b'."

**🤖 AI Agent:**
> I've retrieved the state for aircraft a80c3b. It is currently at an altitude of 35,000ft, traveling at 450 knots, with a heading of 270 degrees.

---

**👤 You:**
> "List all flights departing from Paris Charles de Gaulle (LFPG) in the last 2 hours."

**🤖 AI Agent:**
> I found 12 departures from LFPG in that interval. Notable flights include AF123 to New York and LH456 to Frankfurt. Would you like details on a specific flight?

---

**👤 You:**
> "Show me the trajectory of aircraft '4b1813' for its most recent flight."

**🤖 AI Agent:**
> Fetching the track data for 4b1813... I have retrieved 150 trajectory points showing the climb, cruise, and descent phases of the flight. The path started at Zurich (LSZH) and ended at London (EGLL).


## ❓ FAQ

**Q: How can I see all planes currently flying over a specific area?**
Use the `get_states` tool and provide the geographic bounding box using `lamin`, `lomin`, `lamax`, and `lomax` parameters. The agent will return all active aircraft within those coordinates.

**Q: Can I track the exact path a flight took yesterday?**
Yes. First, identify the aircraft's ICAO24 address, then use the `get_tracks` tool with the specific timestamp to retrieve the full trajectory points of that flight.

**Q: Is it possible to list all flights that arrived at London Heathrow (EGLL) today?**
Absolutely. Use the `get_flights_by_arrival` tool, entering 'EGLL' as the airport and providing the Unix timestamps for the start and end of the day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opensky](https://vinkius.com/mcp/opensky)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenSky** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `opensky` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenSky** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opensky": {
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
