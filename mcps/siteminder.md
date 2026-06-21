# Siteminder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/siteminder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage hotel inventory, search properties, and handle reservations via Siteminder's Channels Plus and Direct Booking APIs.

## Description
Connect your **Siteminder** account to any AI agent to streamline hotel distribution and reservation management through natural conversation.

### What you can do

- **Property Search** — Find properties by location, radius, and dates using Channels Plus (`cp_search_properties`)
- **Inventory & Rates** — Access room types, rates, and quotes for specific properties (`db_get_room_types`, `db_get_room_rates`)
- **Reservation Lifecycle** — Lock, confirm, modify, and cancel bookings directly through the agent (`cp_lock_reservation`, `cp_confirm_reservation`)
- **Booking History** — Retrieve and list historical reservations associated with your account (`cp_list_reservations`)
- **Direct Booking** — List and inspect properties within your group using the Direct Booking API (`db_list_properties`)

### How it works

1. Subscribe to this server
2. Enter your Siteminder API ID, API Key, and SMX Token
3. Start managing hospitality workflows from Claude, Cursor, or any MCP client

### Who is this for?

- **Travel Agencies** — automate property searches and booking confirmations via AI
- **Hotel Managers** — monitor inventory and room rates without manual dashboard checks
- **Developers** — integrate hospitality data into custom workflows or AI assistants


## Available Tools
- **cp_cancel_reservation**: Cancel an existing reservation
- **cp_confirm_reservation**: Finalize booking with guest and payment details
- **cp_get_property**: Get property details via Channels Plus API
- **cp_list_reservations**: Retrieve historical bookings via Channels Plus API
- **cp_lock_reservation**: Create a 10-minute hold on inventory
- **cp_modify_reservation**: Modify an existing reservation
- **cp_search_properties**: Search properties via Channels Plus API
- **db_get_property**: Get property details via Direct Booking API
- **db_get_quotes**: Get pricing and availability for a specific stay
- **db_get_room_rates**: Get room rates for a property via Direct Booking API
- **db_get_room_types**: Get room types for a property via Direct Booking API
- **db_list_properties**: List all properties in the group via Direct Booking API
- **smx_get_availability**: Query inventory for a date range via SMX API
- **smx_get_rates**: Query pricing for a date range via SMX API
- **smx_list_hotels**: List connected properties for a publisher via SMX API
- **smx_list_publishers**: List connected PMS providers via SMX API
- **smx_list_rate_plans**: List rate plans for a hotel via SMX API
- **smx_list_room_types**: List room types for a hotel via SMX API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Siteminder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find hotels near lat 40.7128, long -74.0060 within a 5km radius for next weekend."

**🤖 AI Agent:**
> I've searched the area. I found 3 properties available: 'Grand Plaza' (UUID: gp-123), 'Urban Stay' (UUID: us-456), and 'Boutique Inn' (UUID: bi-789). Would you like to see the room rates for any of these?

---

**👤 You:**
> "Get the room types and rates for property UUID '123-abc-456'."

**🤖 AI Agent:**
> For property '123-abc-456', I found: 'Deluxe King' at $250/night and 'Standard Twin' at $180/night. Both are available for your selected dates. Should I proceed to lock a reservation?

---

**👤 You:**
> "Show me the history of bookings for my account."

**🤖 AI Agent:**
> Retrieving your reservation history... You have 12 recent bookings. The latest is 'RES-99821' for 'John Doe' at 'Grand Plaza', confirmed on Oct 12th. Would you like details on a specific reference ID?


## ❓ FAQ

**Q: How do I search for available hotels in a specific area?**
Use the `cp_search_properties` tool by providing the latitude, longitude, and search radius. You can also include check-in and check-out dates to filter availability.

**Q: Can I hold a room before finalizing a booking?**
Yes! The `cp_lock_reservation` tool creates a 10-minute hold on inventory for a specific property, allowing you to gather guest details before confirming.

**Q: How do I see all properties associated with my account?**
You can use the `db_list_properties` tool to retrieve a full list of all properties in your group via the Direct Booking API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/siteminder](https://vinkius.com/mcp/siteminder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Siteminder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `siteminder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Siteminder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "siteminder": {
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
