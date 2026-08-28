# Lightspeed Restaurant (L-Series) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lightspeed-restaurant-l-series)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage menu items, receipts, floors, tables, customers, and sales for your Lightspeed Restaurant L-Series POS. Note: this connector is for L-Series only — if you use K-Series, use the dedicated Lightspeed Restaurant (K-Series) connector.

## Description
Connect your **Lightspeed Restaurant L-Series** (resto-api) to any AI agent.

### What you can do
- **Menu** — Products with dine-in/takeaway/delivery pricing, SKUs, tax classes, and modifiers
- **Categories** — Product groups with sequence and visibility
- **Receipts** — Today's sales and any date range: items, tips, taxes, and payments
- **Floors & Tables** — Dining rooms, terraces, and table layout with seats
- **Customers** — CRM data, credits, and loyalty cards

> **Which one is mine?** L-Series is the resto-api platform (login at the Restaurant back office). If your credentials come from the K-Series Developer Portal, use the K-Series connector instead.


## Available Tools (14)
- **get_company**: Returns the account's name, address, currency, tax-inclusive flag, opening time, and IANA timezone. The source of truth for the account timezone. Not for sales figures — use get_sales_report or get_product_sales.

Restaurant profile: name, address, currency, tax mode, timezone
- **list_establishments**: Use for multi-location groups. Empty for a single-location account. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data.

Linked locations sharing products and customers
- **get_product_sales**: "from"/"to" are ISO-8601 dates (e.g. 2026-08-01). Use for best-sellers and menu performance. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For the underlying receipts use get_sales_report.

Per-product sales: quantity, revenue, tax, and profit
- **get_receipt**: Returns every item, modifier, tax line, and payment. Get the ID from list_receipts first.

One receipt by ID: full item, tax, and payment breakdown
- **get_sales_report**: "from"/"to" are ISO-8601 (e.g. 2026-08-01T00:00:00). Use for "this week"/"last month" sales. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. Single day → list_receipts; aggregated per-product profit → get_product_sales.

Receipts over a date range: items, totals, tips, payments
- **list_categories**: Use to see how the menu is organized or to group products. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For the products themselves use list_menu_items.

Product groups (menu categories): name, display order, visibility
- **list_clock_times**: Use for hours worked, attendance, or labour tracking. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For staff names/details use list_employees.

Staff clock in/out records per employee
- **list_customers**: Use for CRM, loyalty, or contact lookups. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data.

Customers: name, contact, address, store credit, loyalty cards
- **list_employees**: Use for the roster or to find a person. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For worked hours use list_clock_times.

Staff roster: name, username, email, contact
- **list_floors**: Use for section-level questions. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For a flat list of every table use list_tables.

Floor plans (sections): name, capacity, and their tables
- **list_menu_items**: Use to inspect pricing, find a product, or audit the menu. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. Group by category with list_categories; add-on groups are in list_modifiers.

Menu products: name, price, SKU/PLU, tax class, stock, modifiers
- **list_modifiers**: Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For the products they attach to use list_menu_items.

Modifier groups (add-ons): values, prices, min/max selection
- **list_receipts**: Each: items, modifiers, table, total, tips, payment breakdown, status, type. Optional date (YYYY-MM-DD); defaults to the restaurant's current business day in its own timezone. Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. Multi-day span → get_sales_report; per-product totals → get_product_sales; one receipt by id → get_receipt.

Receipts for one day: items, totals, tips, payments, table
- **list_tables**: Use for table-level questions (how many tables, seats, which section). Paginated: start offset="0", amount="100"; while page.has_more is true, call again with offset=page.next_offset until it is false. You must page to the end for complete data. For the sections themselves use list_floors.

Tables across all floors: number, seats, type, floor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lightspeed Restaurant (L-Series)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What sold today?"

**🤖 AI Agent:**
> Today you have 42 receipts totaling $1,860. Top items: House Burger (18), Caesar Salad (11), Tiramisu (7). Tips collected: $210.

---

**👤 You:**
> "List all menu items with their prices."

**🤖 AI Agent:**
> Here are your menu items: House Burger $6.84, Carpaccio $13.68, Steak $22.39. Want them grouped by category?

---

**👤 You:**
> "Which tables are on the terrace?"

**🤖 AI Agent:**
> The Terrace floor has 3 tables: T-10 (4 seats), T-20 (2 seats), and T-30 (2 seats).


## ❓ FAQ

**Q: What is the difference between L-Series and K-Series?**
They are two separate Lightspeed Restaurant products with completely different APIs. L-Series uses the resto-api (lightspeedapis.com/resto). K-Series uses api.lsk.lightspeed.app. Your credentials only work with the matching connector. This connector is for L-Series.

**Q: How do I get access to the L-Series API?**
Access to the L-Series API is limited to Lightspeed partners and approved developers. You'll need an OAuth client (Client ID + Secret) issued by Lightspeed. Contact your Partner Manager or Lightspeed support to register a client and provide your redirect URI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lightspeed-restaurant-l-series](https://vinkius.com/ai-agent-connect/lightspeed-restaurant-l-series)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lightspeed Restaurant (L-Series)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lightspeed-restaurant-l-series` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lightspeed Restaurant (L-Series)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lightspeed-restaurant-l-series": {
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
