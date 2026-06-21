# Square MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/square)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/square-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/square-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, orders, catalog, customers, inventory, locations, and team members for your Square business through natural conversation.

## Description
Connect your **Square** business to any AI agent — the universal commerce platform.

### What you can do
- **Payments** — Track transactions, tips, refunds, and card processing
- **Orders** — Browse sales with line items, fulfillments, and discounts
- **Catalog** — Menu/product management with pricing and variations
- **Customers** — CRM with visit history, loyalty, and total spend
- **Inventory** — Stock levels, alerts, and cross-location tracking
- **Team** — Employee management with roles and locations


## Available Tools
- **list_team**: List team members
- **get_payment**: Get payment details
- **list_orders**: Core sales tool.

List orders
- **list_payments**: "How much did we take in today?"

List recent payments
- **list_catalog**: List catalog items
- **get_catalog_item**: Get catalog item
- **search_customers**: Returns profile, visit count, total spend, loyalty points, and notes. CRM intelligence.

Search customers
- **get_customer**: Get customer profile
- **list_locations**: List business locations
- **list_inventory**: List inventory counts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Square** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's payments and total tips collected"

**🤖 AI Agent:**
> 🟦 **Today's Payments — Oct 18**

💰 **Total**: $4,230 (67 transactions)
💳 **Card**: $3,890 | 💵 **Cash**: $340
💝 **Tips**: $487 (11.5% avg)

📊 **Breakdown**: Dine-in 72% | Takeout 18% | Delivery 10%

---

**👤 You:**
> "What is the current stock level for medium T-shirts downtown?"

**🤖 AI Agent:**
> 📦 **Inventory Check: Downtown Location**

Item: Logo T-Shirt (Medium)
Current Quantity: **14 units**
Status: Low stock alert (minimum threshold is 15)

---

**👤 You:**
> "Show me a list of my top 5 customers by total spend."

**🤖 AI Agent:**
> 🏆 **Top 5 Customers by Lifetime Spend**

1. Elena Rodriguez — $4,250 (32 visits)
2. Marcus Chen — $3,890 (24 visits)
3. Sarah Jenkins — $3,100 (15 visits)
4. David Smith — $2,750 (18 visits)
5. Liam O'Connor — $2,420 (12 visits)


## Installation & Usage

To install and use the **Square** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/square](https://vinkius.com/mcp/square)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
