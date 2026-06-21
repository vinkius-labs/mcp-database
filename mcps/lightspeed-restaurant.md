# Lightspeed Restaurant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lightspeed-restaurant)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lightspeed-restaurant-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lightspeed-restaurant-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage restaurant orders, menus, tables, employees, payments, and revenue reports for your Lightspeed POS through natural conversation.

## Description
Connect your **Lightspeed Restaurant** to any AI agent — the premium POS for modern restaurants.

### What you can do
- **Orders** — Track tickets, items, modifiers, tips, and voids
- **Menu** — Items, categories, pricing, and availability management
- **Floor Plans** — Dining room, patio, bar sections with table status
- **Payments** — Cash, card, gift cards, and split check tracking
- **Revenue Reports** — Daily gross/net, discounts, taxes, and tips
- **Employees** — Staff roster, roles, clock status, and performance


## Available Tools
- **list_orders**: "What sold in the last hour?"

List restaurant orders
- **get_business**: Get restaurant info
- **get_order**: Get order details
- **list_menu_items**: For menu engineering.

List menu items
- **list_categories**: With item counts and display order.

List menu categories
- **list_floors**: With table count and capacity.

List floor plans
- **list_tables**: List tables
- **list_employees**: List employees
- **list_payments**: List payments
- **get_revenue_report**: The manager daily report.

Get revenue report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lightspeed Restaurant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me the revenue report for today"

**🤖 AI Agent:**
> ⚡ **Revenue Report — Oct 18**

💰 Gross: $6,240 | Net: $5,810 | Discounts: $180 | Taxes: $430 | Tips: $720

---

**👤 You:**
> "Update the price of the Margherita Pizza to $18."

**🤖 AI Agent:**
> I have updated the price of the Margherita Pizza in the dinner menu from $16 to $18. The change is now synced across all active POS terminals.

---

**👤 You:**
> "Which tables are currently available in the patio section?"

**🤖 AI Agent:**
> In the patio section, tables 12, 14, and 15 are currently available and clean. Table 16 is occupied, and table 18 is scheduled for a reservation in 20 minutes.


## Installation & Usage

To install and use the **Lightspeed Restaurant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lightspeed-restaurant](https://vinkius.com/mcp/lightspeed-restaurant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
