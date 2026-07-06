# BookingLive MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bookinglive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate booking and order management via BookingLive — create orders, track statuses, and manage customer reservations directly from your AI agent.

## Description
Connect your **BookingLive** account to any AI agent to streamline your scheduling and commerce workflows. This server enables full control over the booking lifecycle through natural language.

### What you can do

- **Order Lifecycle** — Start new orders, add items to existing ones, and finalize completions with transaction records.
- **Order Retrieval** — Fetch comprehensive metadata for specific order references or filter entire lists by email, status, or creation date.
- **Customer Management** — Instantly retrieve all historical orders associated with a specific purchaser's email address.
- **Order Maintenance** — Cancel or abort orders to keep your inventory clean, and update specific order parameters as requirements change.
- **Availability & Products** — Inspect product details and check resource availability to ensure seamless booking experiences.

### How it works

1. Subscribe to this server
2. Enter your BookingLive Domain and Secret Key
3. Start managing your bookings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — quickly check daily order volumes and status distributions without manual reporting.
- **Customer Support Teams** — find customer order histories and cancel reservations instantly during live chats.
- **E-commerce Leads** — automate the creation and updating of complex booking orders through AI-driven workflows.


## Available Tools (17)
- **complete_order**: Completes an order
- **get_message_content**: Returns the HTML content and subject of an email for a specific order
- **get_order_details**: Returns full details of a specific order
- **get_orders_by_email**: Returns all orders associated with a specific purchaser email
- **get_orders**: Returns a filtered list of all orders
- **get_product_availability**: Returns public product availability for a date range
- **get_product_detail**: Returns details for specific products
- **get_ref_data**: Returns public reference data (Products, ProductGroups, Resources, Locations, Staff)
- **get_resource_availability**: Returns public resource availability for a date range
- **send_email_to_customers**: Sends a specific notification message to a customer
- **set_order_notification**: Sets notification preferences (Email/SMS) for an order
- **start_order**: Provide Member details and OrderItems as JSON objects.

Starts a new BookingLive order
- **update_order_param**: Updates a specific parameter value for an order
- **abort_order**: Aborts an order to ensure no pending items remain
- **add_to_order**: Adds items to an existing order
- **cancel_order**: Cancels an order and sends a cancellation email
- **get_events_by_product_ids**: Returns all events for selected products within a date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BookingLive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all orders associated with the email 'support@example.com'."

**🤖 AI Agent:**
> I found 3 orders for 'support@example.com'. The most recent is REF-9921 (Status: Completed, Total: £45.00). Would you like to see the details for any of these?

---

**👤 You:**
> "Get the full details for order reference BKL-55432."

**🤖 AI Agent:**
> Fetching details for BKL-55432... This order was created on Oct 12th for 'Alice Smith'. It contains 2 items: 'Standard Entry' and 'Equipment Rental'. The total is £60.00 and the status is currently 'Pending'.

---

**👤 You:**
> "Cancel order BKL-1002 and send the confirmation email."

**🤖 AI Agent:**
> Order BKL-1002 has been successfully cancelled. The system has queued the cancellation confirmation email to the customer.


## ❓ FAQ

**Q: Can I search for all orders placed by a specific customer using their email?**
Yes! Use the `get_orders_by_email` tool. Simply provide the customer's email address, and the agent will return a list of all associated orders and their current statuses.

**Q: How do I cancel an existing reservation if a customer changes their mind?**
You can use the `cancel_order` tool by providing the unique order reference. This will cancel the order in the system and trigger the standard cancellation email to the customer.

**Q: Is it possible to view the full transaction history and items for a specific order?**
Absolutely. The `get_order_details` tool fetches everything related to a reference, including totals, transaction types (Cash, PDQ, etc.), order items, and internal notes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bookinglive](https://vinkius.com/mcp/bookinglive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BookingLive** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bookinglive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BookingLive** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bookinglive": {
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
