# Moscow Transit: Metro, Rail, Bus & Parking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/moscow-transit-metro-rail-bus-parking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [smart-city](../categories/smart-city.md)

Keyless Moscow transit: metro and MCD stations (name and line filter), railway stations, bus stops, parking by type and fee, taxi stands, plus transit-system summaries.

## Description
Getting around Moscow, keyless — about 280 metro station areas, 410 railway stations, 12,800 bus stops and 41,000 mapped parking spaces inside the city.

### What you can do
- **find_metro_stations** — every metro and MCD station (about 280) fetched once and filtered locally by name or line — matches full names and line references like "МЦД-1"
- **find_rail_stations** — railway stations (about 410): the nine city terminals, the Central Diameters and suburban stops, with an is_metro flag on shared stations
- **find_bus_stops** — bus and trolleybus stops (about 12,800) by name and proximity
- **find_parking** — parking (about 41,000 mapped spaces) by type — multi_storey, surface, underground, street_side — and fee (free or paid)
- **find_taxi_stands** — mapped taxi stands (about 200)
- **transit_system_facts** — a short Wikipedia entry for a Moscow transit system — the metro, the Central Diameters, the central ring or the surface network

### Who is this for
Anyone moving around Moscow: a visitor finding the right metro line, a driver looking for parking, or an app that needs the city’s transit map.


## Available Tools (6)
- **find_bus_stops**: Each row carries the stop name, the shelter and bench flags, and the coordinate. A name fragment or a proximity search is required in practice — pass lat/km (default 1 km, max 25) around an address or a district centre. Lines and live arrival times are not in the map — use the transit operators' own apps for those.

Find bus and tram stops in Moscow
- **find_metro_stations**: Every station is fetched once and filtered locally, so name and line fragments match against the full list: line holds the mapped line name or reference ("Сокольническая линия", "1", "МЦД-1", "МЦК"). Each row carries the name, the line(s), the wheelchair flag and the centre coordinate. For line overviews use transit_system_facts.

Find Moscow Metro stations
- **find_parking**: Each row carries the name, the parking type (multi_storey, surface, underground, street_side), the fee flag and the centre coordinate. Filter by fee: "no" for free parking, "yes" for paid, or by name fragment (e.g. a shopping centre). A proximity search is the practical way to use this tool.

Find parking in Moscow
- **find_rail_stations**: Metro stations are tagged separately — each row flags is_metro when the map also records it as a subway station, so you can keep or drop the metro with the caller. Filter by name fragment or by proximity to a point.

Find railway stations in Moscow
- **find_taxi_stands**: Each row carries the name, operator and the centre coordinate. A proximity search (lat + km) is the practical way to use this tool — pass a landmark or address coordinate. Ride-hailing apps are not in the map; this is the rank network.

Find taxi stands in Moscow
- **transit_system_facts**: Returns the title, the one-line description and the introductory paragraph, in Russian. For stations on the map use the find_* tools.

Summarise a Moscow transit system (Wikipedia)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moscow Transit: Metro, Rail, Bus & Parking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which metro stations are on the ring line?"

**🤖 AI Agent:**
> find_metro_stations with line: "Кольцевая" returns the stations of the ring line — every station is fetched once and filtered locally, so fragments match full line names.

---

**👤 You:**
> "Where can I park for free near the centre?"

**🤖 AI Agent:**
> find_parking with fee: "no", the centre coordinates and a radius lists the free mapped parking with type and capacity; multi_storey narrows it to garages.

---

**👤 You:**
> "Tell me about the Moscow Central Diameters."

**🤖 AI Agent:**
> transit_system_facts with system: "mcd" returns the Wikipedia summary in Russian; find_rail_stations with name: "МЦД" lists the mapped stations of those lines.


## ❓ FAQ

**Q: Do I need an API key?**
No. Every source is keyless and global: OpenStreetMap (Overpass + Nominatim), Open-Meteo and Russian Wikipedia. The MCP defines no credentials.

**Q: Does it have live arrival times?**
No. The city’s transport portal is not openly reachable from outside Russia, so this is the mapped network — stations, lines, stops — not a real-time feed. Pair it with the official app for live arrivals.

**Q: Why do railway stations carry an is_metro flag?**
Some stations are tagged both as railway=station and station=subway (transfer hubs). The flag lets the caller keep or drop metro overlaps when listing railway stations.

**Q: Can I find parking near a point?**
Pass lat + lon (and optionally km, 0.1–25) and the query narrows to a radius instead of the whole city. Do it before a long list — a citywide scan is capped at 200 rows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/moscow-transit-metro-rail-bus-parking](https://vinkius.com/en/ai-agent-connect/moscow-transit-metro-rail-bus-parking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moscow Transit: Metro, Rail, Bus & Parking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moscow-transit-metro-rail-bus-parking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moscow Transit: Metro, Rail, Bus & Parking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moscow-transit-metro-rail-bus-parking": {
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
