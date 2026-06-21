# HirePOS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hirepos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your hire and rental business with inventory tracking, booking calendars, and invoice generation for equipment providers.

## Description
Connect your **HirePOS** account to any AI agent and manage your equipment rental business through natural conversation.

### What you can do

- **Booking Management** — List all rental hires, create new bookings, filter by status (active, returned, pending, overdue)
- **Inventory Control** — Browse all rental items with rates and categories, check availability for date ranges, and filter by category
- **Customer Database** — List all customers, inspect profiles with rental history, and create new customer records
- **Invoice Processing** — Browse all invoices with amounts and payment status, and inspect individual invoice line items
- **Overdue Tracking** — Identify all rentals past their return date for immediate follow-up
- **Category Management** — Browse all rental item categories for organized inventory

### How it works

1. Subscribe to this server
2. Enter your HirePOS API Key from your account settings
3. Start managing rentals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Rental Business Owners** — manage bookings, track overdue items, and check inventory availability without opening the POS system
- **Operations Staff** — create bookings, check item availability for specific dates, and process customer records
- **Finance Teams** — review invoices, track payments, and audit rental revenue through AI


## Available Tools
- **check_item_availability**: Check item availability
- **check_hirepos_status**: Verify connectivity
- **create_customer**: Create a customer
- **create_hire**: Create a booking
- **get_customer**: Get customer details
- **get_hire**: Get hire details
- **get_invoice**: Get invoice details
- **get_item**: Get item details
- **list_availability**: List availability
- **list_categories**: List categories
- **list_customers**: List customers
- **list_hires_by_status**: Filter hires by status
- **list_hires**: List all hires
- **list_invoices**: List invoices
- **list_items_by_category**: Filter items by category
- **list_items**: List inventory items
- **list_overdue_hires**: List overdue hires


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HirePOS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all overdue rentals and the customer details for each."

**🤖 AI Agent:**
> 3 overdue rentals found. 1) Hire #1045 — 'Excavator CAT 320' rented by BuildCo Pty Ltd (John Smith, john@buildco.com). Due: Apr 20, 2025 (6 days overdue). Daily rate: $450. Estimated late fee: $2,700. 2) Hire #1052 — '2x Concrete Mixers' rented by QuickBuild (Mike Torres). Due: Apr 23 (3 days overdue). 3) Hire #1058 — 'Scaffolding Set A' rented by HomeReno Inc (Sarah Chen). Due: Apr 25 (1 day overdue). Total overdue value: $4,350 in pending late fees. Would you like to view invoices or check these customers' profiles?

---

**👤 You:**
> "Check if the pressure washer is available next week and create a booking for BuildCo."

**🤖 AI Agent:**
> Availability check: 'Pressure Washer 3000 PSI' (item_089) — Available Apr 28 to May 2 ✅. No conflicting bookings. Daily rate: $95. Booking created! Hire #1061, Customer: BuildCo Pty Ltd (cust_012), Items: Pressure Washer 3000 PSI, Period: Apr 28 – May 2 (5 days), Total: $475. Status: Confirmed. Invoice will be generated on return. Would you like to check other equipment availability or view BuildCo's rental history?

---

**👤 You:**
> "List all invoices with unpaid status and the rental items from the 'Power Tools' category."

**🤖 AI Agent:**
> Unpaid invoices: 5 outstanding. 1) INV-2089 — BuildCo, $1,350 (Hire #1045, Excavator). 2) INV-2091 — QuickBuild, $540 (Hire #1052, Mixers). 3) INV-2094 — HomeReno, $280 (Hire #1058, Scaffolding). 4) INV-2095 — GardenPro, $190 (Hire #1060, Mower). 5) INV-2096 — CleanCrew, $475 (Hire #1061, Pressure Washer). Total outstanding: $2,835. Power Tools category: 8 items. Available: Circular Saw ($35/day), Angle Grinder ($25/day), Impact Driver ($20/day), Jigsaw ($15/day). On hire: Drill Press, Router, Planer, Belt Sander.


## ❓ FAQ

**Q: Can I check if a specific item is available for a date range?**
Yes. Use `check_item_availability` with the Item ID, start date, and end date (YYYY-MM-DD format) to verify if the item is free for that period. Use `list_availability` for a complete overview of all items and their current availability status.

**Q: Can I track overdue rentals that haven't been returned?**
Yes. The `list_overdue_hires` tool retrieves all rentals past their return date with customer info, item details, and days overdue. Use `list_hires_by_status` with 'overdue' status for the same result, or filter by 'active', 'returned', or 'pending'.

**Q: Can I create a new rental booking through the AI agent?**
Yes. Use `create_hire` with a JSON payload containing customer ID, item IDs, start date, end date, and any special instructions. Use `list_items` to browse available equipment and `list_customers` to find the customer. Use `create_customer` to add a new customer if needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hirepos](https://vinkius.com/mcp/hirepos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HirePOS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hirepos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HirePOS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hirepos": {
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
