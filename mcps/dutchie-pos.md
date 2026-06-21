# Dutchie POS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dutchie-pos)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage cannabis retail products, track inventory, and monitor orders via the Dutchie POS API.

## Description
Integrate **Dutchie POS** (formerly Greenbits/LeafLogix), the leading retail platform for cannabis dispensaries, directly into your AI workflow. Manage your product catalog and SKUs, track real-time inventory levels and batches, monitor retail orders and fulfillment, and oversee customer loyalty using natural language.

### What you can do

- **Catalog Oversight** — List and retrieve detailed information and SKUs for all your retail products and categories.
- **Inventory Intelligence** — Monitor real-time inventory levels, lot numbers, batch details, and low-stock indicators across your location.
- **Order Management** — Track retail orders, transaction details, payment types, and current fulfillment statuses.
- **Retail Auditing** — Retrieve high-level summaries of sales activity, customer volumes, and organizational metadata instantly.

### How it works

1. Connect the Dutchie POS integration to your AI assistant.
2. Authorize using your Dutchie POS API Key (found in your settings).
3. Orchestrate your dispensary management and retail operations through intuitive conversation.

### Who is this for?

- **Dispensary Managers** — Quickly check inventory levels and daily sales volumes on the go.
- **Inventory Specialists** — Audit stock lots and batch details via chat to ensure compliance.
- **Operations Teams** — Monitor order fulfillment and customer metadata across the organization instantly.


## Available Tools
- **get_dutchie_pos_metadata**: Retrieve metadata and limits for your Dutchie POS account
- **get_order_details**: Get detailed information for a specific order
- **get_product_details**: Get detailed settings and information for a specific product
- **quick_pos_sales_audit**: Retrieve a high-level summary of recent sales activity
- **list_pos_customers**: List all customers registered in your POS organization
- **list_current_inventory**: List all inventory lots and their quantities
- **list_low_stock_inventory**: Identify inventory items that are below a certain quantity threshold (mock logic)
- **list_retail_orders**: List all recent retail orders in Dutchie POS
- **list_retail_products**: List all products in your Dutchie POS catalog
- **search_catalog_products**: Search for products using a name keyword or SKU


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dutchie POS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in the 'Flower' category."

**🤖 AI Agent:**
> I've found 15 products in the Flower category, including 'Blue Dream' and 'Sour Diesel'. Would you like to see the current inventory level for Blue Dream?

---

**👤 You:**
> "Show me our low stock inventory items."

**🤖 AI Agent:**
> The following items are below the threshold: 'Indica Gummies' (3 units left) and 'CBD Tincture' (2 units left). 5 other items are also low. Should I pull the batch numbers for these items?

---

**👤 You:**
> "Check the status of retail order 'ORD-5544'."

**🤖 AI Agent:**
> Order 'ORD-5544' is currently 'FULFILLED'. It was a Cash transaction totaling $125.00 for customer 'John Doe'. Should I list the individual line items for this order?


## ❓ FAQ

**Q: How do I get a Dutchie POS API Key?**
Log in to your Dutchie POS (Greenbits or LeafLogix) back office, navigate to the **Integrations** or **API** section in your settings, and you can generate your unique API Key from there.

**Q: Can the agent update product pricing?**
This integration currently focuses on listing and auditing products, inventory, and orders. Modifying prices or inventory quantities should be managed via the Dutchie POS back office.

**Q: Does it support lab results tracking?**
Yes, you can use the get_product_details tool to retrieve technical metadata which includes batch-level lab result data stored in Dutchie POS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dutchie-pos](https://vinkius.com/mcp/dutchie-pos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dutchie POS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dutchie-pos` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dutchie POS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dutchie-pos": {
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
