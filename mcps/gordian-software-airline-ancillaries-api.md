# Gordian Software (Airline Ancillaries API) MCP Server

Search and book airline ancillaries like seats, bags, and lounge access directly through Gordian Software's API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gordian-software-airline-ancillaries-api)

## Overview
**Category:** payment-processing
**Tools Count:** 17

## Description
Connect to **Gordian Software** to manage airline ancillaries within your AI agent. This server allows you to handle the entire ancillary lifecycle from search to fulfillment through natural language.

### What you can do

- **Trip Management** — Create and update trips with passenger details, currency preferences, and PNR/Record Locator information.
- **Ancillary Search** — Perform asynchronous searches for seats, bags, lounge access, and automatic check-in options across supported airlines.
- **Basket Operations** — Add specific products to a trip basket, check their validity, and manage selections before purchase.
- **Fulfillment** — Finalize the purchase of all valid items in the basket using Gordian settlement or BSP cash payment methods.
- **Real-time Status** — Poll search results and retrieve the current state of any trip, including orders and passenger details.

### How it works

1. Subscribe to this server
2. Enter your Gordian API Key
3. Start booking flight extras through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travel Agencies** — Automate the process of offering and booking ancillaries for clients without manual portal entry.
- **Travel Support Teams** — Quickly check trip states and available products to assist travelers with seat or bag additions.
- **Developers** — Integrate complex airline ancillary workflows into custom travel applications using simple AI commands.


## Available Tools
- **add_to_basket**: Add products to the basket
- **cancel_trip**: Execute the cancellation of a trip
- **check_basket**: Re-validate items in the basket
- **check_cancellation**: Check if items are refundable
- **create_trip**: Can optionally include a search object to start an ancillary search immediately.

Initialize a new trip
- **fulfill_trip**: Payment types: gordian_settlement or bsp_cash.

Initiate the purchase of all valid items in the basket
- **get_basket**: Get current basket items
- **get_refund**: Get refund details for a trip
- **get_search_results_by_product**: g., seat, bag).

Get search results filtered by product type
- **get_search_results**: Contains itineraries and products.

Get search results by search ID
- **get_trip**: Retrieve current trip state
- **inform_cancelled**: Inform Gordian of an external flight cancellation
- **inform_changed**: Inform Gordian of an external flight change
- **request_refund**: Request an airline refund for a ticket
- **start_search**: g., seat, bag).

Start an asynchronous search for specific product types
- **subscribe_callback**: Subscribe to asynchronous event callbacks
- **update_trip**: g., adding a PNR/Record Locator after flight booking).

Update trip details


## Installation & Usage

To install and use the **Gordian Software (Airline Ancillaries API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gordian-software-airline-ancillaries-api](https://vinkius.com/mcp/gordian-software-airline-ancillaries-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
