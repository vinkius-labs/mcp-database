# WooCommerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/woocommerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage products, orders, and store analytics on WooCommerce — the most customizable open-source eCommerce platform.

## Description
Connect your **WooCommerce** store to any AI agent and manage your open-source eCommerce infrastructure through natural conversation.

### What you can do

- **Inventory Discovery** — List and browse your entire product catalog, including prices, SKUs, and stock levels with pagination support
- **Order Management** — Monitor sales by listing orders with status filtering (processing, completed, etc.) and retrieve full billing details
- **Fulfillment Control** — Update order statuses instantly to move items through your shipping and delivery pipelines
- **Customer Insights** — List registered store customers and retrieve deep profile details including total spend and order history
- **Store Analytics** — Retrieve summary sales reports for specific periods (week, month, year) to track business performance
- **Promotion Auditing** — List and browse active discount coupons to monitor promotional campaign performance
- **Deep Metadata** — Access technical product properties and categories to understand your store's taxonomy structure

### How it works

1. Subscribe to this server
2. Enter your WooCommerce Site URL, Consumer Key, and Consumer Secret
3. Start managing your store through Claude, Cursor, or any MCP-compatible client

No more manual logging into WordPress to check an order status. Your AI agent becomes your WooCommerce operations assistant.

### Who is this for?

- **Store Owners** — monitor sales reports and update order statuses on the go through simple chat
- **Operations Managers** — manage inventory levels and audit customer profiles without manual data entry
- **Marketing Teams** — track coupon usage and verify product categories for promotional campaigns
- **Customer Support** — quickly lookup order details and customer billing history to provide rapid assistance


## Available Tools
- **list_store_products**: Lists WooCommerce products with pagination
- **update_order_status**: Statuses: pending, processing, on-hold, completed, cancelled, refunded, failed.

Updates the status of an existing WooCommerce order
- **get_customer_details**: Retrieves details for a specific store customer
- **get_order_details**: Retrieves details for a specific store order
- **get_product_details**: Retrieves details for a specific WooCommerce product
- **get_sales_report**: Period: week, month, last_month, year.

Retrieves a summary sales report for a specific period
- **list_store_categories**: Lists WooCommerce product categories
- **list_store_coupons**: Lists all active discount coupons
- **list_store_customers**: Lists WooCommerce customers with pagination
- **list_store_orders**: Statuses: pending, processing, completed, cancelled, refunded.

Lists WooCommerce orders with pagination and status filtering


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WooCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all processing orders in my WooCommerce store."

**🤖 AI Agent:**
> I found 4 orders currently in 'processing' status: #501 (Total: $120.00), #502 (Total: $45.50), #503 (Total: $89.00), and #504 (Total: $210.00). Would you like to see the shipping address for any of these?

---

**👤 You:**
> "What is the current stock level for product ID '123'?"

**🤖 AI Agent:**
> Product 'Classic T-Shirt' (ID: 123) currently has 15 units in stock. It is assigned to the 'Apparel' category. Would you like me to check other items in this category?

---

**👤 You:**
> "Give me a sales summary for this week."

**🤖 AI Agent:**
> Sales report for this week: You have generated $2,450.00 in total revenue across 32 orders. Your top-selling item was the 'Leather Wallet'. No refunds were processed during this period.


## ❓ FAQ

**Q: Can I check the total sales for the last month via chat?**
Yes. Use the `get_sales_report` tool and specify the period as 'last_month'. Your AI agent will return a summary of your sales performance, including total revenue and order counts for that timeframe.

**Q: How do I update an order's status to 'Completed'?**
You can use the `update_order_status` tool. Provide the unique order ID and set the status to 'completed'. This allows you to manage your fulfillment process directly through conversation.

**Q: Is it possible to see which coupons are being used most in my store?**
Absolutely. The `list_store_coupons` tool retrieves all active discount codes along with their usage counts, helping you identify which promotions are driving the most sales.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/woocommerce](https://vinkius.com/mcp/woocommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WooCommerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `woocommerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WooCommerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woocommerce": {
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
