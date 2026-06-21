# Expedia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/expedia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/expedia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/expedia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate travel planning via Expedia — search hotels, compare flights, find rental cars, and build complete trip itineraries directly from any AI agent.

## Description
Connect your **Expedia Group** developer account to any AI agent and take programmatic control over one of the world's largest travel ecosystems — hotels, flights, and car rentals in a single integration.

### What you can do

- **Hotel Search & Booking** — Find properties by destination, dates, and guest count, then pull room quotes and create bookings directly
- **Flight Discovery** — Search flight routes by origin, destination, and date, then retrieve detailed quotes for specific itineraries
- **Car Rental Lookup** — Query available vehicles at any airport, compare categories, and get pricing quotes
- **Quote Comparison** — Pull detailed pricing breakdowns for hotels, flights, and cars to make data-driven travel decisions
- **Booking Management** — Create and cancel reservations across all travel categories programmatically

### How it works

1. Sign up at the [Expedia Group Developer Hub](https://developers.expediagroup.com/) and create an API project
2. Generate your API Key and API Secret from the developer portal
3. Enter your credentials here and start planning trips from Claude, Cursor, or any MCP-compatible client

Your agent becomes a full-service travel assistant — searching across hotels, flights, and cars without switching between tabs or websites.

### Who is this for?

- **Corporate Travel Managers** — build complete team travel itineraries combining flights, hotels, and ground transport in one conversation
- **Travel Agencies** — automate multi-segment trip research for clients with real-time pricing from a single source
- **Executive Assistants** — plan and modify complex business travel schedules without navigating multiple booking platforms


## Available Tools
- **book_flight**: Book an airline passenger ticket
- **cancel_booking**: Cancel an active property reservation
- **create_booking**: Execute a lodging booking reservation
- **get_car_quotes**: Get active quotes for a rental car class
- **get_flight_quotes**: Get exact real-time pricing for a queried flight
- **get_property_detail**: Get detailed content for a specific property
- **get_room_quotes**: Get live room rates and availability
- **search_cars**: Search for rental cars at specific airport branches
- **search_flights**: Search for airline flights
- **search_properties**: Search for hotels and lodging properties
- **book_car**: Requires driver name and email for confirmation. Returns a booking ID that can be used to manage the reservation. ALWAYS confirm booking details with the user before executing this action.

Book a rental car using a quote ID
- **cancel_flight**: Refund eligibility depends on the fare class and airline cancellation policy. Returns the cancellation status and any applicable refund details. ALWAYS confirm the booking ID and inform the user about potential cancellation fees before executing.

Cancel an existing flight booking
- **search_regions**: Returns region IDs, names, types, and coordinates. This is the essential first step before searching for properties — you need a valid destination identifier from this tool to use search_properties. For example, searching "Paris" returns the city region ID, specific arrondissements, and CDG airport.

Search for geographic regions by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expedia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a complete trip to Tokyo: find hotels near Shibuya for March 10-14, a round-trip flight from LAX, and a rental car at Narita airport."

**🤖 AI Agent:**
> Here's your Tokyo trip plan:

**Hotel:** 'Park Hotel Tokyo' near Shibuya — ¥28,000/night (≈$187), 4.5★, free cancellation until Mar 8. Total: ¥112,000.

**Flight:** LAX → NRT, Delta DL7, departing 11:30 AM, arriving 3:45 PM+1. Economy from $892 round-trip.

**Car:** Compact sedan at Narita — ¥4,200/day ($28) from Toyota Rent a Car, unlimited km.

Estimated total: ~$1,750 for 4 nights. Want me to pull detailed quotes for any of these, or should I book the hotel first?

---

**👤 You:**
> "Compare direct flights from JFK to London Heathrow for next Friday."

**🤖 AI Agent:**
> I found 6 direct flights from JFK to LHR for Friday:

1. **British Airways BA178** — Departs 7:00 PM, arrives 7:05 AM+1, from $684
2. **Delta DL1** — Departs 8:30 PM, arrives 8:40 AM+1, from $712
3. **American AA100** — Departs 10:00 PM, arrives 10:15 AM+1, from $698

BA178 is the best value and has the earliest arrival. Want me to pull a detailed quote with baggage and seat options for any of these?

---

**👤 You:**
> "Get a room quote for property PRO-48291 for two nights starting tomorrow."

**🤖 AI Agent:**
> Here are the room quotes for PRO-48291 (Grand Central Hotel):

**Standard Double** — $189/night, total $378 + $56 taxes. Free cancellation until 6 PM day of check-in.
**Deluxe King Suite** — $279/night, total $558 + $83 taxes. Non-refundable, includes breakfast.

The Standard Double offers the safest option with free cancellation. Would you like me to proceed with booking, or should I search for alternative properties in the area first?


## Installation & Usage

To install and use the **Expedia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/expedia](https://vinkius.com/mcp/expedia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
