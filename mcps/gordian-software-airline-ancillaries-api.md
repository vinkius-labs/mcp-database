# Gordian Software (Airline Ancillaries API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gordian-software-airline-ancillaries-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [payment-processing](../categories/payment-processing.md)

Search and book airline ancillaries like seats, bags, and lounge access directly through Gordian Software's API.

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


## Available Tools (17)
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
- **add_to_basket**: Add products to the basket
- **cancel_trip**: Execute the cancellation of a trip
- **subscribe_callback**: Subscribe to asynchronous event callbacks
- **update_trip**: g., adding a PNR/Record Locator after flight booking).

Update trip details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gordian Software (Airline Ancillaries API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new trip for a passenger in the US using USD and English."

**🤖 AI Agent:**
> I've initialized a new trip. The Trip ID is `trip_8821`. You can now proceed to search for ancillaries or add ticket information.

---

**👤 You:**
> "Search for available seats and bags for trip_8821."

**🤖 AI Agent:**
> I've started the search for seats and bags. The Search ID is `srch_4432`. I will now poll for the results to show you the available options.

---

**👤 You:**
> "Add product_id 'seat_123' to the basket for trip_8821."

**🤖 AI Agent:**
> The seat has been added to your basket for trip_8821. The basket is currently valid. Would you like to fulfill the purchase now?


## ❓ FAQ

**Q: How do I check for available seats or bags for a specific trip?**
First, use the `start_search` tool with your `trip_id` and set `seat_search` or `bag_search` to true. Then, use the `get_search_results` tool with the returned `search_id` to see the available options once the search status is successful.

**Q: Can I update a trip with a PNR after the flight is booked?**
Yes. Use the `update_trip` tool by providing the `trip_id` and a JSON object containing the new fields (like the record locator) to keep your Gordian trip state in sync with your airline booking.

**Q: How do I finalize the purchase of items in the basket?**
Once you have added items using `add_to_basket`, use the `fulfill_trip` tool. You can specify the `payment_type` (e.g., 'gordian_settlement') to initiate the actual purchase process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gordian-software-airline-ancillaries-api](https://vinkius.com/mcp/gordian-software-airline-ancillaries-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gordian Software (Airline Ancillaries API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gordian-software-airline-ancillaries-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gordian Software (Airline Ancillaries API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gordian-software-airline-ancillaries-api": {
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
