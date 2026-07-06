# MarketMan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketman)
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


## Available Tools (8)
- **get_count_sheets**: Get inventory count sheets
- **list_recipes**: For menu engineering.

List recipes
- **get_waste_events**: For waste reduction.

Get waste events
- **get_restaurant_info**: Get restaurant info
- **list_inventory**: "Are we low on anything?"

List inventory items
- **list_purchase_orders**: List purchase orders
- **list_vendors**: For vendor management.

List vendors
- **list_categories**: With item counts.

List inventory categories


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


## ❓ FAQ

**Q: What does MarketMan do?**
MarketMan automates restaurant inventory, purchasing, and food cost management. It integrates with POS systems, accounting software, and suppliers.

**Q: Can MarketMan handle multiple suppliers for the same ingredient?**
Yes, MarketMan allows you to link multiple vendors to a single ingredient, enabling you to compare prices and choose the most cost-effective supplier when generating purchase orders.

**Q: Does the integration track food waste accurately?**
Absolutely. You can log waste events such as spoilage, spills, or over-portioning in MarketMan, and the AI can summarize these events to show you the exact financial impact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketman](https://vinkius.com/mcp/marketman)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MarketMan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marketman` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MarketMan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketman": {
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
