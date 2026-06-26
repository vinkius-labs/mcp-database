# Toast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/toast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage restaurant orders, menus, employees, labor, tables, and payments for your Toast POS through natural conversation.

## Description
Connect your **Toast** restaurant to any AI agent and transform how you run your business.

### What you can do
- **Orders** — Browse today's sales, drill into check details, track voids and comps
- **Menus** — Full menu engineering: items, prices, modifiers, and availability
- **Labor** — Employee rosters, clock-in/out, overtime, and labor cost tracking
- **Tables** — Floor plan, seating status, and section management
- **Payments** — Cash, card, tips, and settlement tracking
- **Revenue Centers** — Bar vs dining room vs patio sales segmentation

### Who is this for?
- **Restaurant Owners** — "How much did we do yesterday?" — instant P&L intelligence
- **General Managers** — Labor cost %, peak hour analysis, and menu performance
- **Chefs** — Menu item popularity, food cost analysis, and 86'd items


## Available Tools (10)
- **list_revenue_centers**: Used for sales segmentation and reporting.

List revenue centers
- **list_dining_options**: With behavior settings and online ordering config.

List dining options
- **list_tables**: For floor plan and seating management.

List restaurant tables
- **list_employees**: For labor management.

List employees
- **list_orders**: THE core tool — "What sold today?"

List restaurant orders
- **get_restaurant**: Get restaurant info
- **get_order**: Deep drill into a single check.

Get order details
- **list_menus**: With categories, availability windows, and ordering channels.

List restaurant menus
- **list_time_entries**: For payroll and scheduling.

List time entries
- **list_menu_items**: "What is our most expensive dish?"

List menu items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Toast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What were our total sales yesterday and what was the most popular item?"

**🤖 AI Agent:**
> 🍽️ **Yesterday's Sales — Oct 17**

💰 **Total Revenue**: $12,847
📊 **Orders**: 234 | **Avg Check**: $54.90

🏆 **Top 5 Items**:
1. 🥩 Grilled Ribeye — 42 sold ($1,638)
2. 🍝 Truffle Pasta — 38 sold ($874)
3. 🍔 Classic Burger — 35 sold ($525)
4. 🥗 Caesar Salad — 31 sold ($403)
5. 🍰 Chocolate Cake — 28 sold ($336)

💡 **Tip**: Ribeye is 12.7% of revenue — consider a weekend special!

---

**👤 You:**
> "Check today's gross sales across all our restaurant locations."

**🤖 AI Agent:**
> Evaluating POS data ('get_sales_summary')...
Here is your gross sales layout for today so far:
- Downtown Location: $4,250.00
- Uptown Location: $3,120.50
- Airport Terminal: $1,400.00
**Total Gross:** $8,770.50.

---

**👤 You:**
> "Update the price of 'Avocado Toast' on the brunch menu to $12.50."

**🤖 AI Agent:**
> Executing `update_menu_item_price` on Toast API...
Item 'Avocado Toast' (ID: menu-items-994) updated successfully.
New Price: $12.50. This syncs to POS devices and online ordering immediately.


## ❓ FAQ

**Q: How many restaurants use Toast?**
Toast powers 112,000+ restaurants in the US — from food trucks and cafes to fine dining and multi-unit chains. It's the #1 restaurant POS platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/toast](https://vinkius.com/mcp/toast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Toast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `toast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Toast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "toast": {
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
