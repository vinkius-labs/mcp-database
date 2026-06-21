# Siteminder MCP Server

Manage hotel inventory, search properties, and handle reservations via Siteminder's Channels Plus and Direct Booking APIs.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/siteminder)

## Overview
**Category:** ecommerce
**Tools Count:** 18

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


## Installation & Usage

To install and use the **Siteminder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/siteminder](https://vinkius.com/mcp/siteminder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
