# NYC Flooding (FloodNet) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-flooding-floodnet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [climate](../categories/climate.md)

Keyless NYC flooding data: DEP FloodNet street-flooding events with depths and durations, plus the flood sensor installation metadata — no API key.

## Description
New York City Department of Environmental Protection (DEP) FloodNet records, keyless.

### What you can do
- **Flood events** — street-flooding events recorded at FloodNet sensors since 2020: start/end times, max depth in inches, onset and drain durations and time spent above 4, 12 and 24 inches
- **Sensors by activity** — the sensors with the most recorded flood events, ranked
- **Sensor lookup** — the installation record for one sensor ID: name, install date, tidal influence, street, borough, geography fields and the lowest-point height delta
- **Sensor list** — the installed sensors citywide (about 500), filtered by borough, NTA, ZIP or tidal influence
- **Events per sensor** — all recorded events for one sensor with its deepest recorded flood

### Who is this for
Flood-risk research, resilience planning, drainage engineering and journalism. Sensor IDs are slugs of the form "BK-richardson-st-n-11th-st-1x59w1" — list_flood_sensors shows installed IDs and names.


## Available Tools (5)
- **flood_events_by_sensor**: The response includes the event count and the deepest recorded flood at that sensor. sensor_id is the full ID slug; lookup_flood_sensor shows installed IDs and their names.

Street-flooding events for one FloodNet sensor
- **list_flood_sensors**: About 500 sensors are installed; filter by borough, NTA or ZIP.

List FloodNet flood sensor locations
- **lookup_flood_sensor**: g. "Brooklyn"), ZIP, community board, council district, census tract, NTA, the lowest-point height delta in inches and coordinates. sensor_id is the full ID slug — list_flood_sensors shows installed IDs and names.

Look up a FloodNet flood sensor installation
- **search_flood_events**: Events have been recorded since 2020 and the dataset is small (a few thousand events) — no date window is applied by default; bound the result with on/after and on/before if needed. Sensor names are of the form "Q - Beach 84 St" (borough-letter prefix + intersection); sensor IDs are slugs (e.g. "BX-ditmars-st-hunter-ave-1kwrk0"). The sensor_name filter is an exact match against the stored name.

Search NYC street-flooding events (FloodNet)
- **top_flood_sensors**: Each row is one sensor name with its event count. Use it to find the most flood-prone monitored locations, then drill in with flood_events_by_sensor or lookup_flood_sensor.

FloodNet sensors with the most recorded flood events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Flooding (FloodNet)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which NYC locations have had the most recorded street floods?"

**🤖 AI Agent:**
> top_flood_sensors returns the sensors ranked by the number of recorded flood events; lookup_flood_sensor then shows where a sensor is and flood_events_by_sensor its recorded events.

---

**👤 You:**
> "How deep did the flood get at the Ditmars St / Hunter Ave sensor?"

**🤖 AI Agent:**
> flood_events_by_sensor with the sensor ID returns every recorded event for that sensor plus its deepest recorded flood; search_flood_events with sensor_name: "Ditmars" finds the events across sensors at that intersection.

---

**👤 You:**
> "Show me the most recent street-flooding events citywide."

**🤖 AI Agent:**
> search_flood_events with no filters returns the events newest first (max depth in inches, onset and drain durations included); add after ("YYYY-MM-DD") to narrow to a period.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: How many FloodNet sensors are installed?**
About 500 sensors are installed citywide and the table of flood events has a few thousand rows recorded since November 2020. list_flood_sensors shows the installed sensors and their IDs; top_flood_sensors ranks them by event count.

**Q: What does a FloodNet sensor ID look like?**
Sensor IDs are slugs of the form "BK-richardson-st-n-11th-st-1x59w1" (borough letter, street intersection and a random suffix). lookup_flood_sensor and flood_events_by_sensor take the full slug; list_flood_sensors shows the installed IDs alongside the human-readable sensor names.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-flooding-floodnet](https://vinkius.com/en/ai-agent-connect/nyc-flooding-floodnet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Flooding (FloodNet)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-flooding-floodnet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Flooding (FloodNet)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-flooding-floodnet": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
