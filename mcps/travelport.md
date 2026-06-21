# Travelport MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/travelport)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access Travelport's Global Distribution System to search and book flights, hotels, and manage travel reservations directly through AI.

## Description
Connect to **Travelport**, the world's leading travel commerce platform, and empower your AI agent to handle complex travel itineraries, real-time flight searches, and hotel bookings.

### What you can do

- **Flight Intelligence** — Search for catalog product offerings, price specific flight legs, and retrieve full pricing details for air offers.
- **Hotel Management** — Search for stays by location or ID, check real-time availability, and retrieve detailed hotel rules and policies.
- **Booking Workbench** — Initialize reservation sessions (workbench), add offers and travelers, and commit bookings to create official PNRs.
- **Payment & Security** — Validate credit cards, verify addresses, and manage payment authorizations directly within the booking flow.
- **Reservation Retrieval** — Fetch existing flight and hotel reservations to provide status updates or itinerary details.

### How it works

1. Subscribe to this server
2. Enter your Travelport credentials (Client ID, Secret, Username, Password, and Access Group)
3. Start searching and booking travel from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agents & Concierges** — Automate the search and booking process for clients using natural language.
- **Corporate Travel Managers** — Quickly retrieve reservation details and check flight availability without manual GDS entry.
- **Developers** — Integrate travel booking capabilities into custom AI workflows and travel assistants.


## Available Tools (21)
- **add_offer_to_workbench**: Add an air offer to an existing workbench
- **add_traveler_to_workbench**: Add a traveler to an existing workbench
- **authorize_card**: Authorize a payment card
- **check_hotel_availability**: Check hotel availability (v11)
- **commit_workbench**: Commit a reservation workbench to create a booking
- **create_hotel_reservation**: Create a hotel reservation (v11)
- **create_workbench**: Create a new reservation workbench session
- **get_hotel_rules**: Get hotel rules (v11)
- **price_offer_full**: Price an air offer fully from products
- **price_offer_reference**: Price an air offer from a catalog reference
- **retrieve_flight_reservation**: Retrieve an existing flight reservation
- **retrieve_hotel_reservation**: Retrieve an existing hotel reservation
- **reverse_authorization**: Reverse a payment card authorization
- **search_flight_specific**: Perform a flight specific search
- **search_flights**: Search for flight catalog product offerings
- **search_next_leg**: Search for the next leg of a flight itinerary
- **search_stays_complete**: Perform a complete hotel search (v12)
- **search_stays_by_id**: Search for hotel properties by ID (v11)
- **search_stays_by_location**: Search for hotel properties by location (v11)
- **validate_card**: Validate a payment card
- **verify_address**: Verify a payment card address (AAVS)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travelport** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for flights from JFK to LHR departing on October 15th and returning on October 22nd."

**🤖 AI Agent:**
> I've found several options for your trip. The best-priced offering is with British Airways at $650. Would you like me to price this specific offer or look for the next leg options?

---

**👤 You:**
> "Find available hotels in Tokyo for a 3-night stay starting tomorrow."

**🤖 AI Agent:**
> Searching Tokyo stays... I found 12 available properties. The 'Park Hyatt Tokyo' has availability starting at $450/night. Shall I check the specific availability and rules for this hotel?

---

**👤 You:**
> "Create a new booking workbench and add traveler John Doe to it."

**🤖 AI Agent:**
> Workbench created successfully (ID: WB-98765). I have added John Doe as the primary traveler. What flight or hotel offer should I add to this session?


## ❓ FAQ

**Q: How do I start a new booking process for a flight or hotel?**
You must first use the `create_workbench` tool to initialize a temporary session. This session allows you to add offers and traveler details before finalizing the booking with `commit_workbench`.

**Q: Can I search for hotels in a specific city or near a landmark?**
Yes! Use the `search_stays_by_location` tool. You can provide geographic coordinates or location criteria to find available accommodations in that area.

**Q: Is it possible to verify a customer's credit card before committing a reservation?**
Absolutely. The server includes `validate_card` and `authorize_card` tools to ensure payment methods are valid and authorized before you proceed with the `commit_workbench` action.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/travelport](https://vinkius.com/mcp/travelport)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travelport** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travelport` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travelport** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travelport": {
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
