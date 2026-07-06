# Clover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage orders, payments, inventory, customers, employees, and discounts for your Clover POS through natural conversation.

## Description
Connect your **Clover** POS to any AI agent — Fiserv-backed commerce platform.

### What you can do
- **Orders** — Track line items, modifiers, tips, and payment status
- **Payments** — Card, cash, refunds, and tip reporting
- **Items** — Product/menu catalog with pricing and tax rates
- **Customers** — Profiles with visit history and total spend
- **Inventory** — Stock levels and reorder alerts
- **Employees** — Staff roster and role management


## Available Tools (10)
- **list_orders**: Core POS tool.

List recent orders
- **get_merchant**: Get merchant info
- **list_items**: List menu/product items
- **list_categories**: List item categories
- **list_customers**: List customers
- **list_employees**: List employees
- **list_payments**: List payments
- **list_inventory**: List inventory
- **list_discounts**: List discounts
- **get_order**: Get order details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's payments breakdown"

**🤖 AI Agent:**
> 🍀 **Today's Payments**

💳 Card: $3,200 (45 txns) | 💵 Cash: $680 (12 txns)
💝 Tips: $380 | ❌ Refunds: $45

---

**👤 You:**
> "List all items running low in stock."

**🤖 AI Agent:**
> Checking Clover inventory... You have 3 items running critically low: 'House Blend Coffee Beans' (2 left), 'Almond Milk Liters' (4 left), and 'Organic Matcha Powder' (1 left).

---

**👤 You:**
> "Find the order receipt for transaction ID #89283."

**🤖 AI Agent:**
> Order #89283 was processed at table 4. Total: $42.50. Items: 2x Cheeseburger, 1x Large Fries, 2x Cola. Payment: Visa ending in 4412.


## ❓ FAQ

**Q: What is Clover?**
Clover is a Fiserv-backed POS platform with dedicated hardware and software for restaurants, retail, and services. One of the largest POS ecosystems globally.

**Q: Does the AI see my real-time inventory count?**
Yes. Upon checking the API inventory endpoints, your agent has exact visibility over product quantities on the floor. It can warn you about low-stock situations instantly.

**Q: Can it issue a customer refund?**
If specifically permitted within your dashboard tokens, yes. The agent can query an order ID and submit a refund command matching the original payment method.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clover](https://vinkius.com/mcp/clover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clover": {
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
