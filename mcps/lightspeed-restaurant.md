# Lightspeed Restaurant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lightspeed-restaurant)
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


## ❓ FAQ

**Q: What is Lightspeed Restaurant?**
Lightspeed is a premium cloud POS platform for restaurants, bars, and cafes — with powerful back-office, analytics, and integrations. Popular in North America, Europe, and Australia.

**Q: Does this integration manage multiple locations?**
Yes, the AI can access data for all locations associated with your main account, allowing you to query menu differences or consolidate revenue reports across venues.

**Q: Can I process payments using natural language?**
While you can track payment types, split checks, and view tip totals, full transaction processing requires direct hardware interaction and is intentionally restricted via the API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lightspeed-restaurant](https://vinkius.com/mcp/lightspeed-restaurant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lightspeed Restaurant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lightspeed-restaurant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lightspeed Restaurant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lightspeed-restaurant": {
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
