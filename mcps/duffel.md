# Duffel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/duffel)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/duffel-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/duffel-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Search and book flights and stays directly through AI. Access real-time offers, manage orders, and explore travel metadata.

## Description
Connect your **Duffel** account to any AI agent to transform it into a powerful travel assistant. Search for flights, book accommodations, and manage travel itineraries through natural conversation.

### What you can do

- **Flight Search & Booking** — Create offer requests, compare prices, and finalize bookings with instant or hold orders.
- **Accommodation (Stays)** — Search for hotels and stays, fetch real-time rates, and get quotes for your next trip.
- **Order Management** — List, retrieve, change, or cancel existing flight orders directly from the chat.
- **Travel Metadata** — Access comprehensive databases of airlines, airports, and aircraft types.
- **Seat Maps & Payments** — View seat configurations and process payments securely.

### How it works

1. Subscribe to this server
2. Enter your Duffel Access Token
3. Start searching and booking travel from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agents & Concierges** — Instantly find the best flight and hotel options for clients without manual portal searching.
- **Corporate Travel Managers** — Manage team bookings, check order statuses, and handle cancellations through a unified AI interface.
- **Developers & Builders** — Integrate travel booking capabilities into custom agents or internal tools with ease.


## Available Tools
- **book_stay**: Book a stay
- **cancel_order**: Cancel a flight order
- **change_order**: Request a change to an existing order
- **create_offer_request**: Create a flight offer request
- **create_order**: Create a flight order (booking)
- **create_payment**: Create a payment for a hold order
- **create_webhook**: Create a webhook
- **fetch_stay_rates**: Fetch all rates for a stay search result
- **get_accommodation**: Get specific accommodation details
- **get_aircraft**: Get a specific aircraft type
- **get_airline**: Get a specific airline
- **get_airport**: Get a specific airport
- **get_offer_request**: Get a specific offer request
- **get_offer**: Get a specific flight offer
- **get_order**: Get a specific flight order
- **get_payment**: Get a specific payment
- **list_accommodation**: List accommodations
- **list_aircraft**: List aircraft types
- **list_airlines**: List airlines
- **list_airports**: List airports
- **list_offer_requests**: List all offer requests
- **list_offers**: List flight offers for a request
- **list_orders**: List all flight orders
- **list_webhook_events**: List webhook events
- **price_offer**: Verify final price and services for an offer
- **quote_stay**: Create a quote for a stay
- **search_stays**: Search for accommodation (Stays)
- **get_seat_maps**: Get seat maps for an offer
- **suggest_accommodation**: Suggest accommodations by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Duffel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for one-way flights from JFK to LHR on October 12th for 1 adult in economy."

**🤖 AI Agent:**
> I've created an offer request (ID: or_0000A...). I found several options, including a direct flight with British Airways for $540 and a Virgin Atlantic flight for $565. Would you like to see the full list of offers?

---

**👤 You:**
> "List my recent flight orders and show me the status of the last one."

**🤖 AI Agent:**
> Retrieving your orders... You have 3 recent orders. The latest one (ID: ord_0000B...) for your trip to Paris is currently 'confirmed'.

---

**👤 You:**
> "Find hotels in Tokyo for check-in on Nov 1st and check-out on Nov 5th for 2 adults."

**🤖 AI Agent:**
> Searching for stays in Tokyo... I found several accommodations. The 'Park Hyatt Tokyo' and 'Shinjuku Prince Hotel' are available for those dates. Should I fetch the specific rates for one of these?


## Installation & Usage

To install and use the **Duffel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/duffel](https://vinkius.com/mcp/duffel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
