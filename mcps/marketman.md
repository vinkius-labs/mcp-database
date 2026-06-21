# MarketMan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketman)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/marketman-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/marketman-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage restaurant inventory, purchase orders, vendors, recipes, food cost, and waste tracking through natural conversation.

## Description
Connect your **MarketMan** account to any AI agent — the restaurant inventory intelligence platform.

### What you can do
- **Inventory** — Real-time stock levels, par levels, and reorder alerts
- **Purchase Orders** — Track vendor orders, deliveries, and invoices
- **Vendors** — Supplier management with order history
- **Recipes** — Ingredient quantities, food cost, and margin analysis
- **Waste** — Spoilage tracking with cost impact
- **Count Sheets** — Inventory counts with variance tracking


## Available Tools
- **list_inventory**: "Are we low on anything?"

List inventory items
- **list_purchase_orders**: List purchase orders
- **list_vendors**: For vendor management.

List vendors
- **list_categories**: With item counts.

List inventory categories
- **get_count_sheets**: Get inventory count sheets
- **list_recipes**: For menu engineering.

List recipes
- **get_waste_events**: For waste reduction.

Get waste events
- **get_restaurant_info**: Get restaurant info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MarketMan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are we low on any inventory items?"

**🤖 AI Agent:**
> 📦 **Low Inventory Alert**

⚠️ **Below Par Level**:
- 🥩 Ribeye: 8 lbs (par: 20) — **ORDER NOW**
- 🧈 Butter: 5 lbs (par: 15) — order by Friday
- 🍋 Lemons: 12 ct (par: 30) — order by Thursday

✅ Everything else is within range (47/50 items OK)

---

**👤 You:**
> "Draft a purchase order for our primary produce vendor."

**🤖 AI Agent:**
> I have prepared a draft purchase order for 'Fresh Farms Inc.' It includes 20 lbs of tomatoes, 15 lbs of onions, and 10 bunches of basil to bring you up to par levels. Total estimated cost is $145. Would you like to review?

---

**👤 You:**
> "What is the current food cost percentage for our signature burger?"

**🤖 AI Agent:**
> The food cost for the Signature Burger is currently at 28.5%. The recent $0.50 increase in beef prices from your wholesale supplier raised the cost per portion by 3%.


## Installation & Usage

To install and use the **MarketMan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketman](https://vinkius.com/mcp/marketman)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
