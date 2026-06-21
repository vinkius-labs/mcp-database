# Saleor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/saleor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/saleor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/saleor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Connect your AI to your headless Saleor e-commerce store. Seamlessly manage products, audit recent orders, and assist customers natively through your chat.

## Description
Empower your conversational AI with deep access to **Saleor**, the highly scalable, headless GraphQL-first e-commerce engine designed around high performance experiences. Connect your environment to actively manage your daily retail store operations, inspect products, or troubleshoot customer inquiries natively from chat.

### What you can do

- **Inventory & Catalogs** — Quickly inspect your store's entire directory (`list_products`). Retrieve detailed specifics such as available variants, pricing, and precise stock configurations per individual product ID (`get_product`).
- **Category Orchestration** — Browse how your catalog is organized internally by fetching collections (`list_collections`) and sub-categories (`list_categories`) without toggling through web dashboards.
- **Order Fulfillment Auditing** — Easily review a list of the latest purchases happening on your platform (`list_orders`) and quickly grab comprehensive snapshots of individual receipts, line items, or billing addresses (`get_order`).
- **Customer Assistance** — Query your database to find registered profiles globally (`list_customers`) or drill down into specific shopper's order details and status natively (`get_customer`).
- **Architecture Inspection** — Inspect high-level configuration such as default currencies and active regions by utilizing `list_channels` or retrieving global details via `get_shop_info`.

### How it works

1. Authorize the Saleor mapping tools within your workspace integrations.
2. Access your main Saleor backend dashboard.
3. Generate a dedicated internal App Token containing adequate reading/managing authorizations.
4. Enter the Saleor Cloud GraphQL API Endpoint and the generated access token simultaneously into the connection securely.
5. Ask the AI: "Find out order specifics and shipping details for order number '334'."


## Available Tools
- **get_customer**: Retrieves profile information and order history for a specific customer
- **get_order**: Retrieves details for a specific order
- **get_product**: Retrieves details for a specific product by ID
- **get_shop_info**: Retrieves global shop configuration
- **list_categories**: Lists all product categories
- **list_channels**: Lists all configured sales channels
- **list_collections**: Lists all product collections
- **list_customers**: Lists all customers/users registered in the shop
- **list_orders**: Lists recent customer orders
- **list_products**: Lists all products in the Saleor store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Saleor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my store."

**🤖 AI Agent:**
> I've carefully queried the Saleor GraphQL endpoint and successfully retrieved the top 20 verified product listings natively currently published within the e-commerce directory mapped accurately here.

---

**👤 You:**
> "Find out order specifics and shipping details for order number '334'."

**🤖 AI Agent:**
> I checked order '334'. It was placed cleanly by 'customer@example.com'. The exact billing address covers CA, and unfortunately the fulfillment standing reveals it's listed strictly as unfulfilled currently.

---

**👤 You:**
> "What currencies does the store utilize in the available sales channels?"

**🤖 AI Agent:**
> I queried the high-level Sales Channels settings securely. You maintain three active pipelines functioning flawlessly: USD for the primary US store, GBP representing the UK environment, and EUR cleanly implemented on the continental node.


## Installation & Usage

To install and use the **Saleor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/saleor](https://vinkius.com/mcp/saleor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
