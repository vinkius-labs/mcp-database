# commercetools MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/commercetools)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/commercetools-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/commercetools-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

commercetools is a flexible, cloud-native e-commerce platform that provides a headless API for composable commerce. This MCP server allows you to manage products, orders, and customer data programmatically.

## Description
Connect your **commercetools** project to any AI agent and manage your composable commerce infrastructure through natural conversation.

### What you can do

- **Catalog Management** — List products, inspect product categories, and query detailed product types across your e-commerce project.
- **Order Processing** — Retrieve recent orders, update order statuses, and inspect purchase histories programmatically.
- **Customer Insights** — Access customer profiles, verify configurations, and extract operational commerce data.
- **Project Administration** — View current project settings, supported languages, currencies, and other essential store configurations.

### How it works

1. Subscribe to this server
2. Enter your commercetools Client ID and Secret (or configured API client token)
3. Start managing your commerce backend through Claude, Cursor, or any MCP-compatible client

No more clicking through the Merchant Center for routine data lookups. Your AI agent integrates directly into your commerce engine.

### Who is this for?

- **E-commerce Managers** — quickly check product availability, monitor recent orders, and troubleshoot missing catalogs.
- **Backend Developers** — inspect API responses directly via chat instead of writing curl scripts or opening Postman.
- **Support Teams** — verify order statuses and customer details in seconds to provide faster assistance.


## Available Tools
- **get_order**: Retrieve detailed information about a specific order
- **get_product**: Retrieve detailed information about a specific product
- **get_project_settings**: Retrieve general settings for the current CommerceTools project
- **list_active_carts**: Retrieve a list of active carts in CommerceTools
- **list_categories**: Retrieve a list of product categories
- **list_customers**: Retrieve a list of customers in CommerceTools
- **list_orders**: Retrieve a list of orders in CommerceTools
- **list_products**: Retrieve a list of products in CommerceTools
- **search_orders_by_number**: Find an order by its order number
- **search_product_by_key**: Retrieve a product by its unique key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **commercetools** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the first 20 products in CommerceTools."

**🤖 AI Agent:**
> I've fetched the first 20 products from your catalog. The list includes 'Classic T-Shirt', 'Denim Jeans', and 'Running Sneakers'. Would you like the SKU details for any of these?

---

**👤 You:**
> "List the last 10 orders in CommerceTools."

**🤖 AI Agent:**
> Here are your latest 10 orders. Order #10452 is 'Confirmed', Order #10451 is 'Shipped', and the rest are 'Complete'. The total revenue from these orders is $1,250.

---

**👤 You:**
> "Show the current settings and languages for my CommerceTools project."

**🤖 AI Agent:**
> Your commercetools project 'my-store-prod' is currently configured to support 3 languages: English (en), Spanish (es), and Portuguese (pt). Supported currencies are USD and EUR.


## Installation & Usage

To install and use the **commercetools** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/commercetools](https://vinkius.com/mcp/commercetools)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
