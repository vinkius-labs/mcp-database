# Bookingmood MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bookingmood)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your rental bookings via Bookingmood — track rentals, manage calendars, and handle guest contacts directly from any AI agent.

## Description
Connect your **Bookingmood** rental management account to any AI agent and orchestrate your availability and booking workflows through natural conversation.

### What you can do

- **Rental Oversight** — List all your rental products and retrieve detailed metadata and descriptions.
- **Booking Management** — Create, update, and manage bookings across your portfolio of rentals.
- **Real-time Availability** — Query and search for available slots and units across specific date ranges.
- **Calendar Synchronization** — Retrieve raw calendar events and blocks to monitor occupancy.
- **Guest Coordination** — Access and manage your guest contact directory and linked bookings.
- **Flexible Querying** — Use PostgREST-powered filters to retrieve exactly the data you need.

### How it works

1. Subscribe to this server
2. Enter your Bookingmood API Key
3. Start managing your rental business from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Property Managers** — quickly check occupancy and manage guest details without manual dashboard work.
- **Vacation Rental Owners** — monitor bookings and availability straight from their workflow tools.
- **Developers** — integrate rental booking data into their custom applications using natural language.


## Available Tools
- **create_booking**: Create a new booking
- **delete_booking**: Delete/cancel a booking permanently
- **get_product**: Get details of a specific rental product
- **list_bookings**: List all current bookings
- **list_calendar_events**: List raw calendar events (blocks)
- **list_contacts**: List guest contacts
- **list_products**: List all rental products
- **query_availability**: Check availability for a list of products
- **search_availability**: Search for available products across dates
- **update_booking**: Update an existing booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bookingmood** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my rental units in Bookingmood."

**🤖 AI Agent:**
> I've retrieved your products. You have 3 rentals active: 'Beachfront Villa' (ID: unit_1), 'Mountain Cabin' (ID: unit_2), and 'City Apartment' (ID: unit_3).

---

**👤 You:**
> "Check availability for 'Beachfront Villa' for the second week of July."

**🤖 AI Agent:**
> Checking availability for 'Beachfront Villa'... It is currently available from July 8th to July 15th. Would you like to create a tentative booking?

---

**👤 You:**
> "Show the last 5 bookings received."

**🤖 AI Agent:**
> Retrieving your recent bookings... I found 5 entries, including a confirmed stay for John Doe at 'Beachfront Villa' starting tomorrow and a pending request for 'Mountain Cabin'.


## ❓ FAQ

**Q: Can I check if a rental is available for a specific weekend?**
Yes! Use the `query_availability` tool with the Product IDs. Your agent will check the real-time calendar status in Bookingmood to confirm if the unit is free or booked.

**Q: How do I see the contact details for a guest with a confirmed booking?**
Simply ask the agent to `list_contacts`. You can filter for specific guests linked to bookings to retrieve their names, emails, and phone numbers directly from the directory.

**Q: Does the integration allow updating the price of a rental?**
The current toolset focuses on availability, booking management, and contact oversight. Updating core pricing calendars or complex rate seasons should be done through the Bookingmood dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bookingmood](https://vinkius.com/mcp/bookingmood)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bookingmood** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bookingmood` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bookingmood** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bookingmood": {
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
