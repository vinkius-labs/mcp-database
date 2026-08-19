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
- **list_modifiers**: For the items they attach to use list_menu_items.

List modifier groups (add-ons)
- **list_employees**: For their worked hours use list_clock_times.

List staff members
- **list_clock_times**: Returns clock-in and clock-out timestamps per employee. For the staff roster/details use list_employees.

List staff clock in/out records
- **list_categories**: Returns product groups with display order and visibility. For the items themselves use list_menu_items.

List menu categories (product groups)
- **list_receipts**: Optional date (YYYY-MM-DD); defaults to the restaurant current business day in its own timezone. Returns each ticket with items, tips, and payments. For a multi-day span use get_sales_report; for per-product totals use get_product_sales.

List receipts (tickets) for one day
- **get_receipt**: Returns the full breakdown: items, modifiers, taxes, and payments. To find the ID first, use list_receipts.

Get one receipt by its ID
- **get_sales_report**: "from" and "to" are required ISO-8601 (e.g. 2026-08-01T00:00:00). Returns the individual receipts in the range. For a single day use list_receipts; for best-sellers/profit per item use get_product_sales.

List receipts over a date range
- **get_company**: Also the authoritative source of the account timezone. Not for sales numbers — use get_sales_report or get_product_sales.

Get restaurant profile and settings
- **list_tables**: For the sections themselves use list_floors.

List all tables across floors
- **list_customers**: For loyalty and marketing lookups.

List customers (CRM)
- **get_product_sales**: "from" and "to" are required ISO-8601 dates (e.g. 2026-08-01). This is the aggregated report; for the raw tickets use get_sales_report.

Get per-product sales analytics
- **list_establishments**: Returns each with name, country, timezone, and tax mode. Empty if the account is a single location.

List linked establishments (locations)
- **list_floors**: For a flat list of tables regardless of section use list_tables.

List floor plans with their tables
- **list_menu_items**: Returns dine-in/takeaway/delivery prices, tax class, stock, and modifiers per item. To group by category use list_categories; for add-on groups use list_modifiers.

List all menu products with prices


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
