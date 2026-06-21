# Ecwid MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecwid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage e-commerce stores via Ecwid — search products and orders, handle inventory, track customers, and audit store profiles directly from any AI agent.

## Description
Connect your **Ecwid by Lightspeed** store to any AI agent and take full control of your e-commerce operations and catalog management through natural conversation.

### What you can do

- **Catalog Orchestration** — Extract explicit catalog nodes evaluating exact pricing constraints and filtering arrays directly to find products by ID or keyword
- **Inventory Management** — Command explicit mutation endpoints dropping rigid inventory payloads to reset physical stock levels and modify literal product states
- **Order Auditing** — List actual completed or pending logical bounds exposing payment constraints, fulfillment statuses, and detailed buyer financial logs
- **Customer Oversight** — Resolve bounded authentication profiles tracking literal historical order arrays and parsing explicit buyer context natively
- **Structural Taxonomy** — Map exact relational taxonomy nodes tracking explicit structural hierarchies properly parsing tree configurations for categories
- **Store Profile Management** — Extract static store globals identifying specific timezone configurations and retrieving precise store formats seamlessly
- **Marketing & Coupons** — Evaluate distinct discounting rules bypassing physical order contexts to check pure coupon boundaries and rules
- **App Data Retrieval** — Request explicit localized string boundaries discovering precise custom payload configurations configured in app storage

### How it works

1. Subscribe to this server
2. Enter your Ecwid Store ID and Secret Automation Token (found in Apps > Develop Apps > App Details)
3. Start managing your online store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Store Owners** — update inventory and monitor orders without opening the Ecwid control panel
- **Inventory Managers** — search for products and update stock levels using natural language
- **Customer Support** — quickly look up order statuses and customer histories to resolve inquiries in real-time
- **Developers** — test and debug e-commerce API parameters and verify product schemas through natural conversation


## Available Tools (10)
- **search_products**: Returns product IDs, names, prices, SKUs, inventory, and images.

Search Ecwid products
- **get_product**: Returns full details: pricing, variations, attributes, choices, and SEO info.

Get Ecwid product by ID
- **search_orders**: Returns order numbers, totals, fulfillment status, payment status, and buyer details.

Search Ecwid orders
- **get_order**: Get Ecwid order by ID/Number
- **search_customers**: Search Ecwid customers
- **list_categories**: List Ecwid product categories
- **get_profile**: Get Ecwid store profile configuration
- **list_coupons**: List Ecwid discount coupons
- **update_inventory**: Update Ecwid product inventory quantity
- **get_app_storage**: Get application storage value from Ecwid by key (useful for custom app state)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ecwid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for products containing 't-shirt' in my store"

**🤖 AI Agent:**
> Searching products... I found 5 items: 'Classic White T-shirt' ($20.00), 'V-Neck Blue T-shirt' ($22.00), etc. Each has inventory and SKU data available. Would you like to check the stock levels for any of these?

---

**👤 You:**
> "Set inventory for product 12345 to 50 units"

**🤖 AI Agent:**
> Inventory updated! Product ID 12345 ('Cotton Polo') is now set to 50 units. The change is live in your store and synced across all channels.

---

**👤 You:**
> "Show me the last 3 orders from yesterday"

**🤖 AI Agent:**
> Retrieving recent orders... I found 3 orders from yesterday: #1001 ($45.00, Paid), #1002 ($120.00, Awaiting Payment), and #1003 ($35.50, Shipped). Would you like to see the customer details for order #1001?


## ❓ FAQ

**Q: Can my agent update product inventory in Ecwid?**
Yes. Use the 'update_inventory' tool. Provide the product ID and the new quantity. The agent will command the Ecwid mutation endpoint to reset the physical stock level perfectly.

**Q: How do I search for orders by a specific customer via chat?**
First, use 'search_customers' to find the buyer details. Then, use 'search_orders' with appropriate filters. Your agent can retrieve the exact financial logs and fulfillment statuses for any order number.

**Q: Can I see all active discount coupons through the agent?**
Absolutely. Use the 'list_coupons' tool. Your agent will evaluate the distinct discounting rules in your account, allowing you to audit coupon boundaries and rules without manual dashboard checks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecwid](https://vinkius.com/mcp/ecwid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ecwid** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ecwid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ecwid** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecwid": {
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
