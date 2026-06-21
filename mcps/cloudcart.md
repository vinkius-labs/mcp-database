# CloudCart MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudcart)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloudcart-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloudcart-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage e-commerce and store operations via CloudCart — track products, monitor orders, and manage customers directly from any AI agent.

## Description
Connect your **CloudCart** account to any AI agent and take full control of your e-commerce operations through natural conversation. Streamline how you manage your product catalog and customer orders natively.

### What you can do

- **Product Oversight** — List and retrieve details for all products in your catalog including SKUs and prices natively
- **Order Intelligence** — Access and monitor customer orders, including fulfillment statuses flawlessly
- **Category Logistics** — List and manage store categories to keep your catalog organized securely
- **Customer Tracking** — Access registered customer profiles and their interaction history flawlessly
- **Abandoned Cart Auditing** — Retrieve a list of abandoned shopping carts to identify recovery opportunities flawlessly
- **Brand Visibility** — List all product brands configured in your store directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your CloudCart Client ID, Client Secret, and Store Domain
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor stock levels and order fulfillment using natural language
- **Store Owners** — audit abandoned carts and customer trends without opening the dashboard
- **Support Teams** — quickly look up order details and customer profiles straight from their chat interface
- **Marketing Teams** — verify product metadata and brand associations across the catalog


## Available Tools
- **get_abandoned_carts**: Retrieve a list of abandoned shopping carts
- **get_order_store_details**: Get detailed information for a specific order
- **get_product_store_details**: Get detailed information for a specific product
- **list_store_brands**: List all product brands configured in the store
- **list_store_categories**: List all product categories in the store
- **list_store_customers**: List all registered customers in the store
- **list_store_orders**: List all customer orders in the store
- **list_store_products**: List all products in the store catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudCart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my CloudCart store."

**🤖 AI Agent:**
> Retrieving your product catalog... I found 5 items: 'Smartphone X' (SKU: SPX-01), 'Laptop Pro' (SKU: LP-2026), and 3 others. Would you like to see the inventory for any of these?

---

**👤 You:**
> "Show me the last 5 orders."

**🤖 AI Agent:**
> Checking recent orders... You have 5 new orders today. #1001 (Processing), #1002 (Shipped), #1003 (Paid), and 2 others. Total revenue from these is $850.00.

---

**👤 You:**
> "What is the status of order ID 'order_98765'?"

**🤖 AI Agent:**
> Retrieving details for order 98765... The order is currently 'Shipped' and was picked up by the courier yesterday. The customer has been notified.


## Installation & Usage

To install and use the **CloudCart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudcart](https://vinkius.com/mcp/cloudcart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
