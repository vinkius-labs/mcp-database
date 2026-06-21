# Commerce7 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commerce7)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/commerce7-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/commerce7-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage wine customers, orders, wine clubs, products, reservations, and inventory for your Commerce7 winery through natural conversation.

## Description
Connect your **Commerce7** winery to any AI agent and run your entire direct-to-consumer business through natural conversation.

### What you can do

- **Customers** — Search by name, email, or phone; view lifetime value, club status, and order history
- **Orders** — Track wine purchases, online orders, club shipments, and POS sales with full line items
- **Wine Clubs** — Manage wine club memberships, allocation tiers, shipment schedules, and member retention
- **Products** — Browse your wine catalog with tasting notes, scores, pricing tiers, and vintage details
- **Reservations** — View tasting room bookings by date with party size, experience type, and host
- **Inventory** — Real-time stock levels: available, allocated, committed, and on-hand
- **Collections & Coupons** — Organize wine catalog categories and manage discount codes

### Who is this for?

- **Winery Owners** — Revenue insights, club health, and DTC performance at a glance
- **Tasting Room Managers** — Daily reservations, walk-in readiness, and VIP guest alerts
- **Wine Club Directors** — Member retention, allocation planning, and shipment coordination
- **Marketing Teams** — Customer segments, coupon performance, and collection merchandising


## Available Tools
- **search_customers**: Returns customer profile, lifetime value, wine club status, order history, and tasting room visits. Essential for DTC relationship management.

Search wine customers
- **list_inventory**: List wine inventory
- **list_collections**: Used for organizing the wine catalog.

List wine collections
- **list_coupons**: With usage limits, expiry dates, and redemption counts.

List active coupons
- **get_customer**: Get customer profile
- **list_orders**: Filter by status: Fulfilled, Processing, Pending. Shows items, totals, and shipping.

List wine orders
- **get_order**: Get order details
- **list_products**: The wine catalog powering ecommerce and POS.

List wine products
- **get_product**: Get wine product details
- **list_clubs**: The backbone of winery DTC revenue.

List wine clubs
- **list_club_members**: List club members
- **list_reservations**: Filter by date for daily planning.

List tasting reservations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commerce7** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many wine club members renewed this month?"

**🤖 AI Agent:**
> 🍷 **Wine Club Report — October 2025**

👥 **Active members**: 1,247
- Reserve Club: 342 (27%)
- Estate Club: 589 (47%)
- Discovery Club: 316 (26%)

📈 **This month**:
- Renewals: 89 members
- New joins: 34
- Cancellations: 12
- Net growth: +22

💰 **Club revenue**: $187,400
📦 **Next shipment**: November 15 (Estate & Reserve)

---

**👤 You:**
> "Show me the details for order number 'ORD-892'."

**🤖 AI Agent:**
> Order #ORD-892. Customer: Jane Doe. Items: 3x Cabernet Sauvignon 2019, 1x Chardonnay 2021. Total: $245.00. Status: Shipped.

---

**👤 You:**
> "Are there any reservations for the tasting room tomorrow?"

**🤖 AI Agent:**
> Yes, you have 4 reservations for tomorrow. Total guests: 12. First reservation is at 11:00 AM (Party of 4, VIP experience).


## Installation & Usage

To install and use the **Commerce7** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commerce7](https://vinkius.com/mcp/commerce7)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
