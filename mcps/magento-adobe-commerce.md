# Magento (Adobe Commerce) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magento-adobe-commerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage e-commerce via Magento (Adobe Commerce) — search products, track orders, and audit customer data.

## Description
Connect your **Magento (Adobe Commerce)** store to any AI agent and take full control of your enterprise e-commerce operations and catalog management through natural conversation.

### What you can do

- **Product Orchestration** — Search and retrieve detailed product metadata by SKU, including pricing, custom attributes, and media galleries directly from your agent
- **Order Monitoring** — List recent commerce orders and retrieve full line-item details, shipping addresses, and status histories securely
- **Customer CRM** — Search for registered customers and retrieve profile data including addresses and group assignments to manage your audience effectively
- **Inventory Audit** — Query real-time stock levels and quantities for specific SKUs to identify shortages and manage supply chain visibility
- **Category Management** — Navigate the entire category tree to understand your store's taxonomy and product distributions across different levels
- **Store Configuration** — Extract store-specific metadata including base URLs, locales, and currency settings to ensure accurate cross-border commerce auditing

### How it works

1. Subscribe to this server
2. Enter your Magento Store URL and Access Token (Integration Token)
3. Start managing your e-commerce platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor order flows and inventory statuses across multiple store views through natural conversation without manual report generation
- **Developers** — verify API responses and audit product attribute mappings directly from your workspace for rapid debugging
- **Store Administrators** — manage customer data and category structures efficiently to maintain a high-performance digital storefront


## Available Tools
- **mg.search_products**: Magento is an enterprise eCommerce platform used by large retailers.

Search Magento/Adobe Commerce products with pagination
- **mg.get_product**: SKU is URL-encoded.

Get Magento product by SKU
- **mg.search_orders**: Use to browse recent commerce orders.

Search Magento orders with pagination
- **mg.get_order**: Needs explicit entity ID.

Get Magento order by ID
- **mg.search_customers**: Search Magento customers with pagination
- **mg.get_customer**: Pass internal customer string ID.

Get Magento customer by ID
- **mg.list_categories**: This might be a very large tree so egress restricts excessive sizes.

List Magento category tree
- **mg.get_stock**: Get Magento stock/inventory for a product SKU
- **mg.list_invoices**: List Magento invoices with pagination
- **mg.get_store_config**: Get Magento store configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magento (Adobe Commerce)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for products containing 'backpack' in the catalog"

**🤖 AI Agent:**
> Searching catalog… I've found several products. Highlights include the 'Adventure Pro Backpack' (SKU: AP-001, $85.00) and the 'Urban Tech Pack' (SKU: UT-005, $120.00). Would you like to see the full details or stock levels for any of these?

---

**👤 You:**
> "Show me the last 5 orders placed today"

**🤖 AI Agent:**
> I've retrieved the latest 5 orders. Highlights: Order #100001 ($45.50, Processing), Order #100002 ($120.00, Pending), and Order #100003 ($15.99, Completed). Would you like to see the customer details for the pending order?

---

**👤 You:**
> "Check the stock level for SKU 'TSHIRT-BLUE-L'"

**🤖 AI Agent:**
> Retrieving stock for 'TSHIRT-BLUE-L'… Currently, you have 45 units in stock. The item is marked as 'In Stock'. Minimum sale quantity is 1 and maximum is 100. Would you like to check other sizes?


## ❓ FAQ

**Q: Can I search for products by SKU through my agent?**
Yes. Use the `mg.get_product` tool and provide the exact SKU. Your agent will fetch the full record, including pricing, stock status, and custom attributes directly from your Magento catalog.

**Q: How do I check the status history of a specific order?**
The `mg.get_order` tool retrieves the complete order entity by ID. Your agent will expose the status history, payment info, and line items, helping you track the fulfillment lifecycle of any order.

**Q: Can my agent list the entire category tree of my store?**
Absolutely. Use the `mg.list_categories` tool to retrieve the complete category hierarchy. Your agent will report the IDs, names, and product counts for each level, ensuring you have a full view of your store's taxonomy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magento-adobe-commerce](https://vinkius.com/mcp/magento-adobe-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Magento (Adobe Commerce)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `magento-adobe-commerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Magento (Adobe Commerce)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magento-adobe-commerce": {
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
