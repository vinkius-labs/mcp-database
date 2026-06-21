# iFood MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ifood)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

AI food delivery: manage orders, menus, and restaurant operations via agents.

## Description
### What you can do

Transform your iFood merchant operations with AI-powered automation. Your agents can:

- **Monitor incoming orders** in real-time with status tracking
- **Accept and progress orders** through preparation workflow
- **Manage restaurant catalogs** — update prices, availability, descriptions
- **Review order details** including customer info, items, and totals
- **Configure operating hours** for each day of the week
- **Track delivery logistics** and assign drivers to orders
- **View store information** and configuration across all locations

### How it works

1. **Connect your iFood merchant account** via JWT token from iFood Developer Portal
2. **Ask your AI agent** to check orders, update menus, or manage schedules
3. **Natural language commands** replace manual app navigation
4. **Automate repetitive tasks** like accepting orders and updating availability

### Who is this for?

Essential for **restaurant owners**, **food delivery managers**, **ghost kitchen operators**, and **multi-location food businesses** using iFood. Let AI agents handle order monitoring, catalog maintenance, and schedule management. Perfect for businesses processing 20+ daily orders who want faster response times, reduced manual oversight, and streamlined operations across multiple store locations.


## Available Tools (11)
- **assign_driver**: Requires order ID and driver ID. Use this to manage your own delivery fleet and coordinate order fulfillment.

Assign a delivery driver to an iFood order
- **get_business_hours**: Use this to review or verify the current schedule before making changes.

Get operating hours for an iFood store
- **get_catalog**: Use this to review menu structure, check item availability, or prepare updates to pricing or descriptions.

Get the menu catalog for an iFood store
- **get_logistics**: Use this to track order fulfillment and coordinate with delivery personnel.

Get logistics/delivery information for an iFood order
- **get_order_details**: Use this to review order contents before accepting or preparing.

Get complete details of a specific iFood order
- **get_orders**: Can filter by status: PENDING, ACCEPTED, PREPARING, READY, DISPATCHED, DELIVERED, CANCELLED. Returns order number, customer info, items, totals, and timestamps. Use this to monitor order flow and track pending orders.

List orders for an iFood store
- **get_store_details**: Use this to review store configuration before making updates.

Get detailed information about a specific iFood store
- **get_stores**: Returns store IDs, names, addresses, and operational status. Use this first to get store IDs needed for other operations like fetching orders or managing catalogs.

List all stores associated with the iFood merchant account
- **update_business_hours**: Requires a schedule object with open/close times for each day. Use this to change store hours, add weekend schedules, or set holiday closures. The schedule should be a JSON object with day keys (monday, tuesday, etc.) and arrays of {start: "HH:MM", end: "HH:MM"} objects.

Update operating hours for an iFood store
- **update_catalog_item**: Only pass the fields you want to change. Common use: update prices, toggle availability, or change descriptions. Requires store ID and item ID.

Update a menu item in the iFood store catalog
- **update_order_status**: Common workflow: PENDING -> ACCEPTED -> PREPARING -> READY -> DISPATCHED -> DELIVERED. Can also set to CANCELLED if needed. Use this to progress orders through the fulfillment pipeline.

Update the status of an iFood order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iFood** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all pending orders and accept them automatically"

**🤖 AI Agent:**
> I'll check your pending orders and accept them right away.

---

**👤 You:**
> "Update the price of 'Combo Burger Especial' to R$32.90 and mark it as unavailable until tomorrow"

**🤖 AI Agent:**
> I'll update the item price and toggle its availability in your catalog.

---

**👤 You:**
> "Change my store hours to open at 11am and close at 11pm every day this week"

**🤖 AI Agent:**
> I'll update your business hours for the entire week right now.


## ❓ FAQ

**Q: Does this work for iFood customers or only merchants?**
This MCP server is designed exclusively for iFood merchants (restaurant owners). It uses the Merchant API to manage orders, catalogs, and operations. Consumer-side features require a different API. If you're a restaurant owner using iFood for delivery, this is for you.

**Q: Can I accept and prepare orders automatically with this MCP?**
Yes! AI agents can update order status through the full workflow: PENDING -> ACCEPTED -> PREPARING -> READY -> DISPATCHED -> DELIVERED. You can build automation rules to accept orders instantly, notify kitchen staff, and track preparation times.

**Q: Does this support multiple restaurant locations?**
Absolutely. The API returns all stores associated with your merchant account. Each tool requires a store_id parameter, so you can manage operations independently across all your restaurant locations. AI agents can list all your stores first to get their IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ifood](https://vinkius.com/mcp/ifood)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iFood** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ifood` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iFood** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ifood": {
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
