# TripGo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tripgo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

AI multimodal transit: plan trips, track vehicles, and check schedules via agents.

## Description
### What you can do

Connect AI agents to the TripGo platform for intelligent multimodal journey planning:

- **Plan trips** combining bus, train, subway, tram, ferry, walking, and cycling
- **Find nearby transit stops** by GPS coordinates with distance and route info
- **Search stops by name** or address for precise location discovery
- **Get real-time departures and arrivals** with live delay estimates
- **Track vehicle positions** on the map with real-time GPS data
- **Review route information** including all stops and agency details
- **Check stop details** with accessibility and amenity information
- **Access global regions** covering major cities worldwide

### How it works

1. **Get your TripGo API key** from developer.tripgo.com (free tier available)
2. **Ask your AI agent** to plan trips, check schedules, or track vehicles
3. **Natural language commands** replace complex transit app navigation
4. **Multimodal planning** combining public transit with active transportation modes

### Who is this for?

Perfect for **urban commuters**, **multimodal travelers**, **cyclists**, **pedestrians**, **transit riders**, **accessibility planners**, and **eco-conscious citizens**. Let AI agents find optimal routes combining buses, trains, bikes, and walking. Ideal for daily commuters who want to compare route options, check real-time departures, track incoming vehicles, and plan sustainable journeys without car dependency.


## Available Tools (9)
- **get_regions**: Each region has an ID, name, and coverage area. Use this first to verify your city is covered before planning trips. Supports major cities across North America, Europe, Australia, and Asia.

List all available transit regions supported by TripGo
- **get_arrivals**: Returns route names, origins, scheduled vs estimated arrival times, and delays. Use this to track incoming vehicles. Requires stop ID.

Get upcoming arrivals to a transit stop
- **get_departures**: Returns route names, destinations, scheduled vs estimated departure times, and delays. Use this to check when your next ride arrives. Requires stop ID.

Get upcoming departures from a transit stop
- **get_nearby_stops**: Returns stop IDs, names, coordinates, routes serving each stop, and distance from search point. Use this to find nearest transit options before planning trips.

Find transit stops near a GPS coordinate
- **get_route_info**: Requires route ID. Use this to understand route coverage before planning trips.

Get information about a specific transit route
- **get_stop_details**: Requires stop ID from nearby stops or search results. Use this to review stop facilities before waiting there.

Get detailed information about a specific transit stop
- **get_vehicle_positions**: Optionally filter by route ID. Use this for real-time tracking of vehicles on the map.

Get real-time vehicle positions for transit vehicles
- **plan_trip**: Combines public transport (bus, train, subway, tram, ferry) with walking and cycling. Returns multiple trip options with departure/arrival times, duration, number of transfers, and step-by-step instructions. Optionally specify travel time and preferred transport modes.

Plan a multimodal trip between two coordinates
- **search_stops**: g., "Times Square", "Main St & 5th Ave"). Returns matching stops with IDs, names, coordinates, routes, and relevance scores. Use this when you know the stop name or intersection but not exact coordinates.

Search for transit stops by name or address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TripGo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a trip from Central Station to Opera House using only public transit and walking"

**🤖 AI Agent:**
> I'll find the best multimodal transit route with walking segments for you.

---

**👤 You:**
> "What buses are departing from Stop 12345 in the next 15 minutes?"

**🤖 AI Agent:**
> I'll check real-time departures for that stop right now.

---

**👤 You:**
> "Show me all train and bus vehicles currently running on Route 480"

**🤖 AI Agent:**
> I'll get real-time vehicle positions for that route on the map.


## ❓ FAQ

**Q: Which cities does TripGo cover?**
TripGo covers major cities worldwide including Sydney, Melbourne, Brisbane, Auckland, Portland, and many more regions. Use the get_regions tool to see the complete list of supported areas. Coverage includes bus, train, tram, ferry, and bike share networks.

**Q: Does TripGo provide real-time transit data?**
Yes! TripGo integrates real-time GTFS-RT feeds where available. The get_departures and get_arrivals tools return both scheduled and estimated real-time arrivals with delay information. Vehicle positions also provide live GPS coordinates when transit agencies broadcast them.

**Q: Can I plan bike-friendly multimodal routes?**
Absolutely! Use the plan_trip tool with modes including 'bike' or 'bicycle' to find routes that combine cycling with public transit. TripGo will suggest bike-friendly paths, bike share stations, and transit connections that accommodate bicycles. Perfect for eco-conscious commuters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tripgo](https://vinkius.com/mcp/tripgo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TripGo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tripgo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TripGo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tripgo": {
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
