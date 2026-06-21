# Cart.com (AmeriCommerce) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cartcom-americommerce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cartcom-americommerce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cartcom-americommerce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

E-commerce store orchestration via Cart.com — manage products, orders, and customers via AI.

## Description
Connect your **AmeriCommerce (Cart.com)** store to your AI agent to unlock professional e-commerce orchestration. From managing product catalogs and tracking inventory to auditing orders and retrieving customer profiles, your agent handles your storefront operations through natural conversation.

### What you can do

- **Product Management** — List, search, and update products in your catalog to ensure your storefront is always current
- **Order Orchestration** — Retrieve incoming orders and update fulfillment statuses seamlessly
- **Customer Intelligence** — List and audit customer profiles to track purchase history and engagement
- **Category Oversight** — Manage product categories to keep your online store perfectly organized
- **E-commerce Insights** — Quickly identify pending orders or low-stock products directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Store Domain and Access Token (Single Token Flow)
3. Start managing your storefront and monitoring sales through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Owners** — automate order audits and monitor inventory levels effortlessly
- **E-commerce Managers** — update product details and manage categories on the fly
- **Customer Support Teams** — quickly look up order statuses and customer history to resolve inquiries
- **Operations Specialists** — retrieve daily sales reports and synchronize data with external tools


## Available Tools
- **list_products**: Supports pagination.

List store products
- **get_product_details**: Get product metadata
- **create_product**: Add a new product
- **list_orders**: List store orders
- **get_order_details**: Get order metadata
- **list_customers**: List customers
- **get_customer_details**: Get customer metadata
- **create_customer**: Add a new customer
- **list_categories**: List product categories
- **get_category_details**: Get category metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cart.com (AmeriCommerce)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pending orders in my store."

**🤖 AI Agent:**
> I've retrieved your orders. You currently have 5 pending orders waiting for fulfillment. Would you like me to retrieve the order items for the most recent one?

---

**👤 You:**
> "Show the details for product ID '1001'."

**🤖 AI Agent:**
> I've retrieved the details for product 1001. It is the 'Premium Coffee Blend'. The current price is $24.99 and you have 150 units in stock. The status is set to active.

---

**👤 You:**
> "Search for a customer with email 'jane.smith@example.com'."

**🤖 AI Agent:**
> I've found the profile for Jane Smith (ID: 555). She has placed 3 orders in the past 6 months and is a member of the 'VIP Customers' group. Would you like to see her recent order history?


## Installation & Usage

To install and use the **Cart.com (AmeriCommerce)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cartcom-americommerce](https://vinkius.com/mcp/cartcom-americommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
