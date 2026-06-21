# eCellar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecellar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage premium winery customers, orders, wine clubs, products, reservations, and inventory for your eCellar DTC platform through natural conversation.

## Description
Connect your **eCellar** winery to any AI agent and manage your premium DTC operation through natural conversation.

### What you can do

- **Customers** — Search by name, email, or phone; view lifetime spend, club status, and tasting room history
- **Orders** — Track online, tasting room, phone, and club shipment orders with full line items
- **Wine Clubs** — Manage membership tiers, allocation, and shipment schedules
- **Products** — Browse your wine catalog with pricing, tasting notes, and stock levels
- **Reservations** — View and manage tasting room bookings by date
- **Inventory** — Real-time stock across all locations: available, allocated, and on-hand

### Who is this for?

- **Premium Winery Owners** — Revenue dashboards, club health, and VIP customer insights
- **Tasting Room Teams** — Daily reservation prep and guest recognition
- **Wine Club Directors** — Member retention and allocation planning
- **Operations** — Multi-location inventory and fulfillment tracking


## Available Tools
- **search_customers**: Returns profile, lifetime spend, wine club membership, tasting room visits, and purchase history. Core CRM data for personalized wine recommendations.

Search wine customers
- **list_inventory**: Multi-location inventory management.

List wine inventory
- **get_customer**: For VIP identification and personalized service.

Get customer profile
- **list_orders**: With line items, totals, payment, and fulfillment status.

List wine orders
- **get_order**: Get order details
- **list_products**: The product catalog powering ecommerce and POS.

List wine catalog
- **get_product**: Get wine details
- **list_clubs**: Essential for DTC revenue planning.

List wine clubs
- **list_club_members**: For retention and engagement tracking.

List club members
- **list_reservations**: Filter by date for daily planning.

List tasting reservations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eCellar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who are our top 5 customers by lifetime spend?"

**🤖 AI Agent:**
> 🍷 **Top 5 Customers — Lifetime Value**

1. **Michael & Sarah Henderson** — $47,200
   - Reserve Club member since 2018
   - 23 tasting room visits
   - Last order: Oct 2 (6x Estate Cab 2021)

2. **Jennifer Park** — $38,900
   - Founder's Circle since 2016
   - Prefers Bordeaux blends

3. **David & Lisa Chen** — $34,100
   - Estate Club, 18 visits

4. **Robert Williams** — $31,500
   - Reserve Club, corporate events

5. **Amanda Torres** — $28,700
   - Discovery Club → upgraded to Reserve 2024

---

**👤 You:**
> "Search for inventory levels of the 2019 Reserve Cabernet."

**🤖 AI Agent:**
> The 2019 Reserve Cabernet Sauvignon currently has 240 bottles on-hand at the main warehouse and 48 bottles available in the Tasting Room. 24 bottles are currently allocated for upcoming club shipments.

---

**👤 You:**
> "Show me the reservation schedule for tomorrow afternoon."

**🤖 AI Agent:**
> You have 12 reservations booked for tomorrow afternoon between 1:00 PM and 5:00 PM, totaling 45 guests. There are two VIP members arriving at 2:00 PM (the Hendersons and Robert Williams).


## ❓ FAQ

**Q: How is eCellar different from Commerce7?**
eCellar is an all-in-one DTC platform popular with ultra-premium Napa Valley and Sonoma wineries. It includes CRM, ecommerce, POS, wine clubs, and reservations in a unified system with full REST API.

**Q: Does this integration require additional licensing from eCellar?**
No, the Exchange REST API is generally available to all eCellar customers. You simply need to request your unique API Key and Secret from the eCellar support team as mentioned in the instructions.

**Q: Can I manage reservations with this tool?**
Yes! The integration provides full access to your reservation and booking systems, allowing you to quickly query upcoming visits, manage guest lists, and track tasting room capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecellar](https://vinkius.com/mcp/ecellar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eCellar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ecellar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eCellar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecellar": {
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
