# Cin7 Core MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cin7-core)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cin7-core-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cin7-core-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage inventory, sales orders, and purchase orders via the Cin7 Core (formerly DEAR Systems) API.

## Description
Integrate **Cin7 Core** (formerly **DEAR Systems**), the advanced cloud-based inventory management platform, directly into your AI workflow. Manage your product catalog, monitor real-time stock levels, track sales and purchase orders, and research customer and supplier data using natural language.

### What you can do

- **Inventory Intelligence** — List and retrieve detailed information for products and check real-time stock availability across warehouses.
- **Order Management** — Monitor sales and purchase orders, track their status, and access full fulfillment details.
- **CRM & Supplier Research** — Quickly access customer and supplier profiles and their historical interactions.
- **Multi-warehouse Oversight** — Track inventory locations and stock movement efficiently via chat.

### How it works

1. Connect the Cin7 Core integration to your AI assistant.
2. Authorize using your Account ID and Application Key (found in your Cin7 Core/DEAR API settings).
3. Orchestrate your inventory and commerce operations through intuitive conversation.

### Who is this for?

- **Inventory Managers** — Quickly check stock levels and product locations on the go.
- **Operations Teams** — Monitor order fulfillment and purchase statuses via chat.
- **Sales & Purchasing Reps** — Research customer and supplier details during planning sessions.


## Available Tools
- **get_product_details**: Resolves detailed attributes such as dimensions, weight, supplier info, and tax rules for the given product GUID.

Get detailed information for a specific product by ID
- **get_sale_order_details**: Resolves individual line items, shipping addresses, invoice details, and the current fulfillment progress.

Get full details for a specific sales order
- **get_sku_stock_status**: Provides a detailed breakdown of quantities across all physical locations and virtual bins.

Get stock levels for a specific product SKU
- **get_all_stock_availability**: Returns real-time availability data including on-hand, allocated, and available-to-sell quantities across all configured warehouse locations.

Retrieve current stock availability across all warehouses
- **list_crm_customers**: Returns customer metadata including contact names, company details, and credit limits.

List all customers registered in the system
- **list_inventory_products**: Returns a list of products with metadata including SKU, name, category, and base price.

List all products in your Cin7 Core (DEAR) catalog
- **list_purchase_orders**: Returns a list of purchase orders including supplier details, order date, and inbound status (e.g., ordered, received).

List all purchase orders and inbound shipments
- **list_sales_orders**: Returns order metadata including customer ID, total value, and current status (e.g., drafted, authorized, packed, shipped).

List all sales orders and their current fulfillment status
- **list_crm_suppliers**: Returns vendor profiles including primary contact info, default currency, and payment terms.

List all suppliers and vendors
- **search_products_by_sku**: Returns stock and identification data for products matching the provided SKU identifier.

Search for a product using its SKU


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cin7 Core** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the stock level for product SKU 'CH-1001'?"

**🤖 AI Agent:**
> Product SKU 'CH-1001' (Premium Leather Chair) currently has 45 units available across all locations. 30 units are in the 'Main Warehouse' and 15 are in 'Distribution Center B'. Should I check if there are any pending sales orders for this SKU?

---

**👤 You:**
> "List all sales orders that are currently 'Awaiting Fulfillment'."

**🤖 AI Agent:**
> I've found 12 sales orders awaiting fulfillment, including 'Order #SO-123' for 'Alpha Corp' and 'Order #SO-124' for 'Beta Industries'. Would you like to see the details for the largest order by value?

---

**👤 You:**
> "Show me the contact details for supplier 'Furniture Pros'."

**🤖 AI Agent:**
> I've retrieved the profile for 'Furniture Pros'. Your main contact is 'Jane Smith' (jane.smith@furniturepros.com). They currently have 2 active purchase orders with us. Should I list their recent order history?


## Installation & Usage

To install and use the **Cin7 Core** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cin7-core](https://vinkius.com/mcp/cin7-core)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
