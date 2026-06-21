# Line-Up MCP Server

Manage events, check ticket availability, and process bookings via the Line-Up API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/line-up)

## Overview
**Category:** event-management
**Tools Count:** 10

## Description
Connect your **Line-Up** account to any AI agent to automate your event ticketing and booking workflows. This MCP server enables your agent to list active events, check real-time ticket availability for specific performances, and manage customer orders directly from natural language interfaces.

### What you can do

- **Event Discovery** — List all available events and retrieve detailed metadata, descriptions, and schedules
- **Inventory Check** — Query specific performances to check real-time availability across various ticket categories
- **Reservation Flow** — Programmatically create temporary ticket holds and reservations for customers
- **Order Management** — Confirm bookings, retrieve order histories, and monitor transaction statuses
- **Customer CRM** — List and inspect customer profiles and their historical booking data
- **Operational Auditing** — Access comprehensive logs of all confirmed orders within your portal

### How it works

1. Subscribe to this server
2. Enter your Line-Up API Key and Subdomain
3. Start managing your ticketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — Monitor ticket sales and event availability via simple natural language commands
- **Box Office Staff** — Quickly retrieve order details and customer profiles without leaving your productivity tools
- **Developers** — Integrate event booking logic and inventory monitoring into your custom applications


## Available Tools
- **confirm_ticket_order**: Requires a JSON body.

Finalize a booking and create an order
- **create_ticket_reservation**: Requires a JSON body.

Reserve tickets temporarily
- **list_ticket_customers**: List all customers in the database (Admin)
- **list_available_events**: List all events available for booking
- **get_customer_profile**: Get details for a specific customer
- **get_event_details**: Get details for a specific event
- **get_order_details**: Get details for a specific order
- **list_account_orders**: List all historical orders (Admin)
- **list_event_performances**: List specific dates and times (performances) for an event
- **check_ticket_availability**: Check ticket types and availability for a performance


## Installation & Usage

To install and use the **Line-Up** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/line-up](https://vinkius.com/mcp/line-up)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
