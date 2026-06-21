# Kibo Commerce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kibo-commerce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce catalogs, orders, and real-time inventory via Kibo Commerce.

## Description
Connect your **Kibo Commerce** account to any AI agent to automate your enterprise e-commerce operations. This MCP server enables your agent to interact with products, inventory, orders, and customer accounts directly through natural language.

### What you can do

- **Catalog Management** — List products and categories, and retrieve detailed metadata for your entire catalog
- **Inventory Visibility** — Get real-time stock levels and availability for any product across all locations
- **Order Oversight** — List and inspect commerce orders, including statuses and fulfillment details
- **CRM Access** — Query customer accounts and profile data registered in your tenant
- **Infrastructure Tracking** — List physical locations (stores/warehouses) and retrieve site settings

### How it works

1. Subscribe to this server
2. Enter your Tenant ID, Client ID, and Client Secret
3. Start managing your e-commerce platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — Monitor order statuses and catalog updates without opening the admin panel
- **Inventory Specialists** — Quickly verify stock levels across locations via natural language
- **Customer Support** — Retrieve customer details and order history instantly during interactions


## Available Tools (10)
- **list_categories**: List all catalog categories
- **list_customers**: List all customer accounts
- **get_location_details**: Get details for a specific location
- **get_order_details**: Get details for a specific order
- **get_product_details**: Get details for a specific product
- **get_inventory_status**: Get real-time inventory for a product
- **list_locations**: List all inventory locations (stores/warehouses)
- **list_orders**: List all commerce orders
- **list_products**: Use this to explore your inventory and item metadata.

List all products in the Kibo catalog
- **get_site_settings**: Get platform site settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kibo Commerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the details for product with code 'TSHIRT-RED-XL' in Kibo."

**🤖 AI Agent:**
> I've retrieved the details for 'TSHIRT-RED-XL'. It's a 'Classic Red V-Neck T-Shirt' in size XL. Current status is 'ACTIVE' and it has 5 associated attributes.

---

**👤 You:**
> "What is the inventory status for product 'LAPTOP-PRO-15'?"

**🤖 AI Agent:**
> For 'LAPTOP-PRO-15', I found 120 units on hand across 3 locations: Warehouse-A (80 units), Store-Downtown (25 units), and Store-Westside (15 units).

---

**👤 You:**
> "List my 5 most recent orders in Kibo Commerce."

**🤖 AI Agent:**
> I've fetched your latest orders. Notable recent ones include Order #1005 from 'Alice Smith' ($150.00) and Order #1004 from 'Bob Jones' ($85.50).


## ❓ FAQ

**Q: Can I check stock levels for a specific location?**
Yes, the `get_inventory_status` tool provides stock levels for a product across all registered locations in your tenant.

**Q: Is it possible to list all current commerce orders?**
Absolutely. Use the `list_orders` tool to retrieve a comprehensive list of recent orders and their current processing status.

**Q: How do I find physical store locations via the agent?**
The `list_locations` tool retrieves all physical and logical locations (stores, warehouses, etc.) configured in your Kibo inventory system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kibo-commerce](https://vinkius.com/mcp/kibo-commerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kibo Commerce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kibo-commerce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kibo Commerce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kibo-commerce": {
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
