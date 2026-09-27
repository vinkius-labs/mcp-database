# NYC Cycling & Bike Infrastructure MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-cycling-bike-infrastructure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless NYC cycling data: bike route segments and named greenways, bike racks and secure corrals, and live bike, pedestrian and scooter sensor counts — no API key.

## Description
New York City cycling infrastructure and traffic, keyless. Built for trip planning — where the protected lanes and greenways are, where to lock a bike, and how busy a corridor is right now.

### What you can do
- **Bike route segments** — the ~29,700 segments of the city's signed/marked bike routes with street, from/to streets, direction code, facility classification ("Protected", "Conventional", "Shared", ...) and greenway, by boro (name or code 1-5), street (auto-uppercased), classification or greenway
- **Greenway rankings** — the named greenways ("Manhattan Waterfront", "Jamaica Bay", "Brooklyn Waterfront", ...) ranked by segment count; the unmarked majority sits in the top row
- **Segment count** — a fast count of route segments matching a filter
- **Bike parking** — the ~38,000 chainable racks and secure/community corrals with address and street, by boro, program or street
- **Corral list** — the 912 secure and community bike corrals only
- **Top sensors** — the busiest bike, pedestrian or scooter sensors by total counts in a lookback window (default 90 days, max 365), with street context via the flowname of search_bike_flows
- **Direction split** — the in/out volume split for a travel mode over a window, to read commuter direction
- **Sensor readings** — raw 15-minute interval counts (bike/pedestrian/scooter, in/out) in a lookback window, filterable by sensor id, direction or the street-context flowname; the count data is live, collected up to today

### Who is this for
Cyclists and visitors planning bike trips across the city: trace protected lanes street by street, find a corral to leave a bike for hours, and check how busy a bridge or boulevard corridor is before riding. Every text filter is an exact match on the stored value: the route table stores streets UPPERCASE and the parking table mixes casings, so pass the street as it appears in a result row.


## Available Tools (8)
- **bike_direction_split**: Compare the two rows to see which way a corridor carries more traffic, e.g. the commuter bias on the bridges into Manhattan.

Inbound vs outbound split for a travel mode
- **count_bike_lanes**: ) or named greenway. A single fast count — use it to gauge how large a list_bike_lanes call will be, e.g. to confirm how many protected-lane segments a street has.

Count NYC bike route segments matching a filter
- **list_bike_corrals**: Filter by boro or by the stored street value. Use it when planning where to leave a bike for hours, as opposed to the chainable racks in search_bike_parking.

List secure and community bike corrals
- **list_bike_lanes**: g. "1 AV"), the from/to streets, the on/off streets, the direction code ("L", "R" or "2" for two-way), the facility classification — "Protected", "Conventional", "Shared", "Signed Route", "Wide Parking Lane", "Sidewalk" or "Curbside" (most segments are unclassified and come back null) — and the greenway it belongs to when marked. About 29,700 segments; most recently updated segments first. The street filter is an exact UPPERCASE stored value, auto-uppercased. Use it to trace the route network street by street, for planning a bike trip across the city.

List NYC bike route segments
- **search_bike_flows**: Each row is one 15-minute interval count with the sensor id, the travel mode ("bike" by default), the direction ("in" or "out"), the flowname — the street or intersection context, e.g. "87th ST. and Columbus IN" — the timestamp, the count and whether the value is raw or modified. Filter by sensor id, direction or flowname (exact stored value, e.g. "Manhattan Bridge Display Bike Counter Cyclist IN"). Hourly summary readings are excluded; the count data is live, collected up to today.

Search raw traffic sensor readings
- **search_bike_parking**: g. "Brooklyn"), the program ("Bike Racks", the 37,000+ chainable racks, or "Bike Corral", the 912 secure or community corrals with a BCxxxx group id), the site id, the full address and the street it sits on with its from/to streets. About 38,000 sites citywide. The boro filter is auto-title-cased; the program filter is an exact value; the street filter matches the stored street casing exactly (the table mixes casings, e.g. "BROADWAY" and "Broadway"), so pass it as it appears in a result row. Use it to find where a visitor can lock a bike near an attraction.

Search NYC bike racks and corrals
- **top_bike_greenways**: The top row is the unmarked majority — about 24,000 of the 29,700 segments are not on a named greenway — so a greenway's true length is the number of rows below that first one. Use it to see which protected multi-use greenways make up the city's long-distance cycling corridors.

Rank named NYC bike greenways by segment count
- **top_bike_sensors**: Each row is one sensor id (numeric) with its summed counts — the sensors publish 15-minute interval tallies, so the sum approximates how many cyclists, pedestrians or scooters passed in the window. To get street context for a sensor, call search_bike_flows with that sensor id: the flowname carries the location, e.g. "87th St. and Columbus IN" or "Manhattan Bridge Display Bike Counter Cyclist IN". The count data is live, collected up to today.

Top bike, pedestrian or scooter sensors by volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC Cycling & Bike Infrastructure** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where are the protected bike lanes on First Avenue in Manhattan?"

**🤖 AI Agent:**
> list_bike_lanes with boro: "Manhattan" and street: "AV" (auto-uppercased to "1 AV" context aside) — pass the street as stored, e.g. street: "1 AV" — plus facilit_type: "Protected" returns the protected-lane segments on that street with their from/to streets and direction code.

---

**👤 You:**
> "How busy is the bike traffic on the Williamsburg Bridge right now?"

**🤖 AI Agent:**
> top_bike_sensors with days: "30" ranks the busiest bike sensors; then search_bike_flows with that sensor id returns the recent 15-minute readings with the flowname (e.g. "Williamsburg Bridge Bike Path [Bike IN]"), so you can read the current volumes per direction.

---

**👤 You:**
> "Where can I leave a bike for hours in Manhattan?"

**🤖 AI Agent:**
> list_bike_corrals with boro: "Manhattan" returns the secure and community bike corrals in Manhattan (about a third of the city's 912 corrals) with their address, site id and the street they sit on — the places to keep a bike locked for hours, unlike the chainable racks.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Do the text filters ignore case or match partial values?**
No. The NYC data platform only supports exact-match filters, and each table stores its values differently: the bike-route table stores the boro as the numeric code 1-5 and the street in UPPERCASE ("1 AV" — the tool auto-uppercases the street input); the bike-parking table stores the boro in title case ("Brooklyn", "Staten Island") and mixes street casings (e.g. "BROADWAY" and "Broadway" — pass the street as it appears in a result row). Facility classifications are stored as "Protected", "Conventional", "Shared", "Signed Route", "Wide Parking Lane", "Sidewalk" or "Curbside", and the greenway names are a short set ("Manhattan Waterfront", "Jamaica Bay", "Brooklyn Waterfront", ...). Use list_bike_lanes or search_bike_parking with no filters to see the exact stored values before filtering.

**Q: What do the direction codes on bike routes mean?**
The route segments carry a short direction code: "L" for left-side/one-way, "R" for right-side/one-way and "2" for two-way operation. Use it to read which way a one-way street's bike lane flows.

**Q: How do sensor ids map to streets?**
top_bike_sensors returns numeric sensor ids. Call search_bike_flows with that sensor id: the flowname field carries the street context, e.g. "87th ST. and Columbus IN" or "Manhattan Bridge Display Bike Counter Cyclist IN". Only 15-minute interval readings are returned (hourly summary rows are excluded), and the counts are live, collected up to today.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-cycling-bike-infrastructure](https://vinkius.com/en/ai-agent-connect/nyc-cycling-bike-infrastructure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC Cycling & Bike Infrastructure** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-cycling-bike-infrastructure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC Cycling & Bike Infrastructure** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-cycling-bike-infrastructure": {
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
