# InflatableOffice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inflatableoffice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Run your party rental and inflatable business with online booking, inventory management, and delivery route planning.

## Description
Connect your **InflatableOffice** account to any AI agent and manage your party rental business through natural conversation.

### What you can do

- **Lead Management** — List all leads, inspect details, and create new leads for potential customers
- **Inventory Tracking** — Browse all rental equipment (inflatables, tables, chairs, etc.) with pricing and availability
- **Customer Database** — List all customers with contact information and rental history
- **Event Scheduling** — Monitor all scheduled events with dates, equipment, and delivery details

### How it works

1. Subscribe to this server
2. Enter your InflatableOffice Public Key from your account settings
3. Start managing rentals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Rental Business Owners** — manage leads and events without opening the POS
- **Sales Teams** — track leads and follow up on bookings
- **Operations** — monitor inventory availability and scheduled deliveries


## Available Tools (6)
- **create_new_lead**: Register a new lead
- **get_lead_details**: Get details for a specific lead
- **list_customers**: List InflatableOffice customers
- **list_scheduled_events**: List scheduled events
- **list_rental_inventory**: List rental inventory
- **list_leads**: List InflatableOffice leads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **InflatableOffice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all leads and the upcoming scheduled events for this weekend."

**🤖 AI Agent:**
> Leads: 12 active. Hot (3): Johnson Birthday Party ($450), Martinez Graduation ($680), Smith Corporate Event ($1,200). Warm (5). Cold (4). Weekend events: 4 scheduled. Sat: 'Johnson Birthday' — 2 bounce houses, 1 slide. Delivery 9 AM. 'Garcia Wedding' — tent, tables, chairs. Sun: 'Community Fair' — 5 inflatables. 'Park Fundraiser' — 3 units. Total weekend revenue: $3,200.

---

**👤 You:**
> "Create a new lead for a corporate event and show the rental inventory."

**🤖 AI Agent:**
> Lead created! Company: TechCorp Annual Picnic. Contact: David Williams, david@techcorp.com. Date: May 15. Budget: $2,500. Status: Hot. Rental inventory: 45 items. Inflatables: Bounce Houses (8, from $150/day), Slides (4, from $200), Obstacle Courses (3, from $350). Tents: 10x10 ($75), 20x20 ($150), 30x30 ($300). Tables & Chairs: Round tables ($15), folding chairs ($2). Currently available: 38 of 45.

---

**👤 You:**
> "Show all customers and their rental history."

**🤖 AI Agent:**
> Customers: 156 total. Top by revenue: 1) Johnson Family — 8 events, $3,400 lifetime. 2) Martinez Events — 5 events, $2,800. 3) Smith Corp — 3 events, $2,100. Recent customers: Garcia Wedding (new, 1 event). Community Center (recurring, 12 events). Average lifetime value: $425. Repeat rate: 42%. Would you like to create a lead or check events?


## ❓ FAQ

**Q: Can I manage leads and create bookings through the AI agent?**
Yes. Use `list_leads` to see all leads, `get_lead_details` for full profiles, and `create_new_lead` to add potential customers. Use `list_scheduled_events` to see all bookings.

**Q: Can I check equipment availability and pricing?**
Yes. `list_rental_inventory` retrieves all equipment with pricing, categories, and current availability status. This includes inflatables, tables, chairs, tents, and other party rental items.

**Q: How does InflatableOffice authentication work?**
InflatableOffice uses a **Public Key** passed as a query parameter (`?public_key=YOUR_KEY`) in all requests to `inflatableoffice.com/api2/`. This is different from Bearer token authentication.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inflatableoffice](https://vinkius.com/mcp/inflatableoffice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **InflatableOffice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inflatableoffice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **InflatableOffice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inflatableoffice": {
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
