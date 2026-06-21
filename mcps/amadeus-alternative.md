# Amadeus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amadeus-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your travel planning — audit flight offers, hotels, and destinations via AI.

## Description
Empower your AI agent to orchestrate your entire travel planning workflow with **Amadeus**, the global leader in travel technology. By connecting Amadeus to your agent, you transform complex logistics searches into a natural conversation. Your agent can instantly search for flight offers, audit hotel availability, and retrieve points of interest without you ever touching a booking site. Whether you are organizing a business trip or scouting vacation destinations, your agent acts as a real-time travel consultant, ensuring your itineraries are always optimized and data-driven.

### What you can do

- **Flight Auditing** — Search for real-time flight offers between any cities and retrieve detailed pricing and itinerary metadata.
- **Hotel Oversight** — Browse hotel options in specific cities and retrieve detailed offer metadata for any hotel ID.
- **Destination Discovery** — Query points of interest and recommended locations based on geographic coordinates to plan perfect stays.
- **Travel Intelligence** — Retrieve seat maps and direct destination data from any airport to maintain strict control over logistics.
- **Pricing Insights** — Query the cheapest flight dates and destinations from an origin to optimize your travel budget.

### How it works

1. Subscribe to this server
2. Enter your Amadeus API Key and API Secret
3. Start managing your travel intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Coordinators** — monitor flight options and hotel availability straight from your workflow.
- **Digital Nomads** — verify cheapest destinations and flight dates without manual searching.
- **Event Planners** — perform rapid audits of points of interest near venues through natural language.
- **Operations Leads** — automate travel logistics querying to orchestrate cross-functional teams smoothly.


## Available Tools (10)
- **get_direct_destinations**: Get direct destinations from an airport
- **get_flight_dates**: Get cheapest flight dates
- **get_flight_destinations**: Get flight destinations from an origin
- **get_hotel_offers**: Get specific offers for a hotel ID
- **get_travel_recommendations**: Get recommended locations based on coordinates
- **get_seat_map**: Get seat map for a flight offer ID
- **search_cities**: Search for cities and locations
- **search_flights**: Search for flight offers
- **search_hotels**: Search for hotels by city code
- **search_poi**: Search for points of interest


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amadeus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for flights from NYC to LON on 2024-12-01 for 1 adult."

**🤖 AI Agent:**
> I've retrieved 5 flight offers. The cheapest one is a direct flight with British Airways for $550. Would you like the full itinerary or seat map options?

---

**👤 You:**
> "Find hotels in 'MAD' (Madrid)."

**🤖 AI Agent:**
> I've found 10 hotels in Madrid. Top-rated options include 'Westin Palace' and 'Hotel Ritz'. I can provide the specific offer IDs for these hotels if you'd like.

---

**👤 You:**
> "Show points of interest near latitude 48.8584, longitude 2.2945."

**🤖 AI Agent:**
> I've identified several POIs near those coordinates, including the Eiffel Tower and Trocadéro Gardens. Would you like more details or nearby recommendations?


## ❓ FAQ

**Q: How do I find my Amadeus API Key and Secret?**
Log in to your [**Amadeus for Developers dashboard**](https://developers.amadeus.com/), create a new Self-Service App, and you will find your API Key and Secret under the 'API Keys' section. Copy and paste them below.

**Q: Does this work with real booking data?**
This server default connects to the Amadeus Test API environment. To use production data, ensure your credentials are from a production app in the Amadeus dashboard.

**Q: Can the agent search for hotels in a specific city?**
Yes. Use the `search_hotels` tool providing the City IATA code (e.g., 'PAR' for Paris). Your agent will retrieve matching hotels instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amadeus-alternative](https://vinkius.com/mcp/amadeus-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amadeus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amadeus-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amadeus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amadeus-alternative": {
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
