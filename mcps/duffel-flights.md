# Duffel Flights MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/duffel-flights)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search and book flights via Duffel — list airlines, airports, and manage flight orders directly via AI.

## Description
Connect your AI agent to **Duffel**, the modern infrastructure for travel. This integration allows you to search for real-time flight offers, manage bookings (orders), and access a comprehensive directory of airlines, airports, and aircraft through natural conversation.

### What you can do

- **Flight Search** — Create offer requests to find the best flights based on origin, destination, dates, and cabin class
- **Booking Management** — Create flight orders (instant or hold) and retrieve detailed reservation information
- **Payment Processing** — Pay for flight orders that were previously held directly via the agent
- **Travel Directory** — List and inspect aircraft models, airlines, and airports worldwide with their respective IATA codes
- **Order Oversight** — List all flight bookings associated with your account to track your travel history

### How it works

1. Subscribe to this server
2. Enter your **Duffel Access Token** (obtained from the Duffel Dashboard)
3. Start searching and booking travel directly through natural language

### Who is this for?

- **Travel Agencies** — quickly search for offers and manage client bookings via AI assistance
- **Corporate Travel Managers** — oversee company flight orders and airport metadata
- **Travel Enthusiasts** — research flight options and track reservation statuses without leaving the chat


## Available Tools
- **create_flight_offer_request**: Provide passengers as a JSON array string.

Search for flight offers by specifying origin, destination, and passengers
- **create_flight_order**: Provide full passenger details as a JSON string.

Book a flight by selecting an offer and providing passenger details
- **pay_for_flight_order**: Process payment for a flight order that was previously put on hold
- **list_aircraft**: Retrieve a list of aircraft used by airlines
- **list_airlines**: Retrieve a list of airlines
- **list_airports**: Retrieve a list of airports
- **list_flight_offers**: Retrieve all available flight offers for a specific offer request
- **list_flight_orders**: Retrieve a list of all flight bookings (orders)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Duffel Flights** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a flight from London (LHR) to New York (JFK) on 2024-12-01."

**🤖 AI Agent:**
> Creating offer request... I found several options, including a direct flight with British Airways for $550. Would you like to see the full list of offers?

---

**👤 You:**
> "List all airports in Brazil."

**🤖 AI Agent:**
> Retrieving airports... I found major hubs including Guarulhos (GRU), Congonhas (CGH), and Galeão (GIG). Would you like the ICAO codes for any of them?


## ❓ FAQ

**Q: How do I get a Duffel Access Token?**
Sign up for a developer account at the [**Duffel Dashboard**](https://app.duffel.com/). You can generate both 'test' tokens for development and 'live' tokens for real bookings.

**Q: Can I make real bookings with this agent?**
Yes, if you provide a 'live' access token, the agent can perform real flight bookings. We recommend using a 'test' token first to understand the search and booking flow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duffel-flights](https://vinkius.com/mcp/duffel-flights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Duffel Flights** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `duffel-flights` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Duffel Flights** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "duffel-flights": {
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
