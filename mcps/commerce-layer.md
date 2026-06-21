# Commerce Layer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commerce-layer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/commerce-layer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/commerce-layer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Enable your AI agent to manage orders, SKUs, customers, and shipments via the Commerce Layer API.

## Description
Connect your AI assistant to **Commerce Layer**, the headless commerce API and order management system built for multi-market operations.

### What you can do

- **Order Management** — List recent orders, filter by status, and inspect individual order details including line items and payment info.
- **SKU Lookup** — Search for products by SKU code and retrieve pricing, inventory levels, and metadata.
- **Customer Data** — Find customers by email, list their order history, and check associated addresses.

### How it works

1. Add the Commerce Layer integration to your AI toolset.
2. Provide your organization subdomain, Client ID, and Client Secret.
3. Query your commerce data via natural language commands.

### Who is this for?

- **E-commerce Managers** — Check order statuses and SKU availability without navigating the admin dashboard.
- **Customer Support** — Quickly find a customer's orders by email to resolve inquiries faster.
- **Developers** — Inspect API resources and debug order flows directly from chat.


## Available Tools
- **get_order**: Retrieve details of a specific order
- **get_order_stats**: Calculate basic stats for a set of orders
- **get_sku**: Retrieve details of a specific SKU
- **list_customers**: Retrieve a list of customers
- **list_orders**: Retrieve a list of orders from Commerce Layer
- **list_prices**: Retrieve a list of product prices
- **list_skus**: Retrieve a list of SKUs (products)
- **list_shipments**: Retrieve a list of shipments
- **search_orders_by_email**: Find orders belonging to a specific customer email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commerce Layer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 orders in Commerce Layer."

**🤖 AI Agent:**
> Here are your 10 most recent orders:
1. #ORD-4521 — $89.99 (Fulfilled, Jan 22)
2. #ORD-4520 — $142.50 (Pending, Jan 21)
3. #ORD-4519 — $35.00 (Cancelled, Jan 20)
Would you like details on any of these?

---

**👤 You:**
> "Find the SKU 'TSHIRT-BLUE-L' and show its details."

**🤖 AI Agent:**
> SKU: **TSHIRT-BLUE-L**
- Name: Blue T-Shirt (Large)
- Price: $29.99
- Stock: 142 units available
- Weight: 200g
Would you like to check inventory across all markets?

---

**👤 You:**
> "Find the customer with email 'jane.doe@example.com'."

**🤖 AI Agent:**
> Customer found:
- Name: Jane Doe
- Email: jane.doe@example.com
- Total Orders: 5
- Lifetime Value: $650.00
Shall I display her recent order history?


## Installation & Usage

To install and use the **Commerce Layer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commerce-layer](https://vinkius.com/mcp/commerce-layer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
