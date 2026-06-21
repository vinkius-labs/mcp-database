# eCellar MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecellar)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ecellar-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ecellar-mcp)
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


## Installation & Usage

To install and use the **eCellar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecellar](https://vinkius.com/mcp/ecellar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
