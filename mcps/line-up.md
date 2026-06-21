# Line-Up MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/line-up)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Manage events, check ticket availability, and process bookings via the Line-Up API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Line-Up** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events in my Line-Up account."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 active events: 'Summer Music Festival', 'Tech Conference 2024', and 'Art Gallery Opening'. Which one would you like to check availability for?

---

**👤 You:**
> "Check ticket availability for performance ID 'perf-123'."

**🤖 AI Agent:**
> I've checked the availability for performance perf-123. Currently, 'VIP Tickets' has 15 remaining and 'Standard Admission' has 120 available.

---

**👤 You:**
> "Show the 5 most recent confirmed orders."

**🤖 AI Agent:**
> I found 5 recent orders. Notable ones include Order #ORD-987 from 'John Smith' ($150.00) and Order #ORD-986 from 'Alice Doe' ($75.00).


## ❓ FAQ

**Q: How do I check if tickets are available for a specific date?**
First, use `list_event_performances` to get the performance ID for your target date, then use `check_ticket_availability` with that ID to see current stock.

**Q: What is required to confirm an order?**
You typically need to create a reservation first using `create_ticket_reservation`, then provide the resulting reservation data to the `confirm_ticket_order` tool.

**Q: Where do I find my API Key?**
Log in to your Line-Up dashboard and navigate to Settings > API to generate and copy your Secret API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/line-up](https://vinkius.com/mcp/line-up)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Line-Up** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `line-up` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Line-Up** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "line-up": {
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
