# Wix eCommerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wix-ecommerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage products, orders, and inventory on Wix — the complete eCommerce platform for growing online businesses.

## Description
Connect your **Wix eCommerce** store to any AI agent and manage your online business infrastructure through natural conversation.

### What you can do

- **Product Catalog** — Browse and filter your entire product list, including prices, variants, and gallery images
- **Order Management** — Monitor sales in real-time, retrieve full order details, and list abandoned carts for recovery analysis
- **Inventory Control** — Check stock levels for multiple product IDs and manually update quantities for specific variants
- **Fulfillment Tracking** — Mark orders as shipped and manage fulfillment records with tracking numbers directly from your agent
- **Collection Access** — List all product collections and categories to understand how your inventory is organized
- **Sales Auditing** — Retrieve billing addresses, payment totals, and line item breakdowns for any order ID
- **Business Insights** — Quickly find unique site and product IDs required for automated eCommerce workflows

### How it works

1. Subscribe to this server
2. Enter your Wix API Key and Site ID
3. Start managing your store through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex store dashboards to check a stock level. Your AI agent becomes your eCommerce operations manager.

### Who is this for?

- **Store Owners** — automate inventory updates and monitor daily sales performance through chat
- **Operations Teams** — manage order fulfillments and track shipments without manual data entry
- **Marketing Managers** — analyze abandoned carts and verify product details for upcoming campaigns
- **Customer Support** — quickly lookup order statuses and customer details to provide rapid assistance


## Available Tools (10)
- **create_order_fulfillment**: Provide the order ID and tracking number.

Creates a new fulfillment record with tracking for an order
- **get_order_details**: Retrieves details for a specific store order
- **get_product_details**: Retrieves full details for a specific Wix product
- **list_product_collections**: Lists all product categories/collections in the store
- **list_order_fulfillments**: Lists all fulfillment records for a specific order
- **list_abandoned_carts**: Lists recent abandoned carts for recovery analysis
- **query_stock_inventory**: Provide a comma-separated list of product IDs.

Checks inventory levels for specific product IDs
- **list_store_orders**: Queries recent eCommerce orders
- **query_products**: Returns product IDs, names, and prices.

Lists and filters products in the Wix store
- **update_stock_quantity**: Provide the inventory item ID and the new total quantity.

Updates the inventory quantity for a specific product variant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wix eCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 orders in my Wix store."

**🤖 AI Agent:**
> I found your 5 most recent orders: 1. #1005 (Total: $45.00, Status: PAID), 2. #1004 (Total: $120.00, Status: FULFILLED), 3. #1003 (Total: $89.99, Status: PAID), and 2 others. Would you like the full details for any of these?

---

**👤 You:**
> "What is the current inventory level for product 'Coffee Mug'?"

**🤖 AI Agent:**
> Checking inventory for 'Coffee Mug' (ID: prod-mug-123)… You have 42 units in stock across all variants. Would you like me to update the quantity for any specific variant?

---

**👤 You:**
> "Create a fulfillment for order #1005 with tracking number 'TRACK12345'."

**🤖 AI Agent:**
> Success! I've created a fulfillment record for order #1005. The order status has been updated to 'Fulfilled' and the tracking number TRACK12345 has been added. The customer will be notified.


## ❓ FAQ

**Q: Can I check which products are running low on stock via chat?**
Yes. The `query_stock_inventory` tool allows your AI agent to check real-time stock quantities for specific product IDs, helping you identify items that need restocking without manual auditing.

**Q: How do I mark an order as shipped and add a tracking number?**
You can use the `create_order_fulfillment` tool. Simply provide the order ID and the tracking number, and your agent will update the Wix order status and record the shipment details instantly.

**Q: Can I see details for abandoned carts to help with recovery?**
Absolutely. The `list_abandoned_carts` tool retrieves a list of recent checkout sessions that weren't completed, showing you which products were left behind so you can plan recovery strategies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wix-ecommerce](https://vinkius.com/mcp/wix-ecommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wix eCommerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wix-ecommerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wix eCommerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wix-ecommerce": {
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
