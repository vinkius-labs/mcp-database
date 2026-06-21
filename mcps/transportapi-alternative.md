# TransportAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transportapi-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

UK public transport intelligence — live departures, journey planning, train fares, timetables, and postcode-based station search via AI.

## Description
Empower your AI agent to orchestrate your entire public transport research workflow with **TransportAPI**, Britain's leading platform for transport data. By connecting TransportAPI to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly search for stations, audit live bus and train departures, and retrieve detailed journey plans without you ever touching a travel app. Whether you are conducting urban mobility research or monitoring daily commute patterns, your agent acts as a real-time transit consultant, ensuring your data is always comprehensive and up-to-date.

### What you can do

- **Departure Auditing** — Query real-time bus and train departures for any stop or station to maintain a clear view of local transit flow.
- **Journey Oversight** — Plan public transport routes between any locations and retrieve detailed itinerary metadata, including aimed vs expected times.
- **Station Discovery** — Search for train stations and bus stops by keyword or retrieve nearby transport hubs based on geographic coordinates.
- **Service Intelligence** — Query specific bus and train service details, including operator information and full route timetables.
- **Logistics Monitoring** — List available routes and service statuses to maintain strict control over urban transport data.

### How it works

1. Subscribe to this server
2. Enter your TransportAPI App ID and API Key
3. Start managing your transport intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Urban Researchers** — monitor public transport patterns and retrieve live transit metadata straight from your workflow.
- **Logistics Managers** — verify service reliability and audit operator performance across different lines.
- **Daily Commuters** — perform rapid audits of nearby departures and identify the best routes through natural language.
- **Operations Leads** — automate transport data querying to orchestrate cross-functional mobility teams smoothly.


## Available Tools
- **get_bus_service**: Get details of a bus service route
- **get_bus_route_timetable**: Get the scheduled timetable for a bus route
- **get_transport_by_postcode**: Useful when user only has a postcode, not coordinates.

Find transport options by UK postcode
- **get_live_bus_departures**: Returns live departure times, destinations, and operators.

Get real-time bus departures for a UK bus stop
- **get_live_train_departures**: g., KGX for King's Cross, PAD for Paddington).

Get real-time train departures for a UK station
- **get_nearby_bus_stops**: Find bus stops near a GPS location
- **get_nearby_transport_places**: Find transport locations near GPS coordinates
- **get_train_fares**: Great for price comparison.

Get ticket prices between two stations
- **get_train_service_details**: Get the full calling pattern of a train service
- **get_train_station_timetable**: Get the scheduled timetable for a train station
- **plan_public_transport_journey**: Returns step-by-step route with times and changes.

Plan a public transport journey between two locations
- **search_transport_places**: Search for train stations and bus stops by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TransportAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show live train departures for station 'EUS' (Euston) using TransportAPI."

**🤖 AI Agent:**
> I've retrieved the live departures for London Euston. Notable trains include the service to Manchester Piccadilly at 10:20 and Birmingham New Street at 10:35. Would you like the platform numbers?

---

**👤 You:**
> "Plan a journey from 'London Waterloo' to 'Brighton'."

**🤖 AI Agent:**
> Journey plan retrieved! The best route is a direct train from Waterloo, taking approximately 1 hour and 10 minutes. I can provide the full list of intermediate stops and aimed departure times.

---

**👤 You:**
> "Search for bus stops near coordinate 51.5074, -0.1278."

**🤖 AI Agent:**
> I've identified several bus stops near Charing Cross. Notable stops include 'Trafalgar Square' and 'Horse Guards Parade'. Would you like the live departures for any specific stop ATCO code?


## ❓ FAQ

**Q: How do I find my TransportAPI credentials?**
Log in to your [**TransportAPI dashboard**](https://developer.transportapi.com/), and you will find your App ID and App Key under your 'Account' or 'Apps' section. Copy and paste them below.

**Q: Does this cover transport outside of the UK?**
TransportAPI provides high-density data primarily for the UK transport network, including national rail, London Underground, and regional bus services.

**Q: Can the agent plan a journey from coordinates?**
Yes. Use the `get_journey_plan` tool providing coordinates in 'lat,lon' format for the 'from' or 'to' parameters. Your agent will calculate the best public transport route instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transportapi-alternative](https://vinkius.com/mcp/transportapi-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TransportAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `transportapi-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TransportAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transportapi-alternative": {
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
