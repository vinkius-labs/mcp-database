# Jumpseller MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jumpseller)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jumpseller-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jumpseller-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage products, orders, and customers via Jumpseller API.

## Description
Empower your AI agents with Jumpseller's e-commerce platform. This MCP server allows you to list and retrieve products and orders, manage customers and categories, track store pages, and view general store information directly through the Jumpseller API. Ideal for automating store management and order processing.


## Available Tools
- **get_order**: Returns line items, shipping addresses, payment status, and customer notes. Use this for order troubleshooting or providing customer support.

Retrieves details for a specific order
- **get_product**: Returns descriptions, detailed pricing, variants, and image metadata. Use this when the user needs to analyze a specific item or prepare product listings.

Retrieves details for a specific product
- **get_store_info**: Useful for verifying store configuration.

Retrieves general information about your Jumpseller store
- **list_categories**: Useful for understanding store organization and finding products within specific niches.

Lists all product categories
- **list_customers**: Returns names, emails, and order counts. Use this when the user wants to identify repeat buyers or audit the customer list.

Lists all customers in your store
- **list_orders**: Includes order IDs, totals, and current fulfillment status. Essential for monitoring recent sales activity.

Lists all orders in your store
- **list_pages**: ) from the Jumpseller store. Useful for auditing site content and navigation.

Lists all pages in your store
- **list_payment_methods**: g., PayPal, Stripe) in the store. Useful for auditing checkout options.

Lists configured payment methods
- **list_products**: Returns product names, SKUs, prices, and IDs. Use this to identify items for stock management or product analysis.

Lists all products in your Jumpseller store
- **list_shipping_methods**: Useful for auditing fulfillment logic and carrier configurations.

Lists configured shipping methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jumpseller** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active products in my Jumpseller store."

**🤖 AI Agent:**
> I'll fetch the complete list of products from your Jumpseller account.

---

**👤 You:**
> "Show me the last 5 orders received."

**🤖 AI Agent:**
> I'll retrieve the most recent orders from your store for you.

---

**👤 You:**
> "Check the details for customer ID '123'."

**🤖 AI Agent:**
> I'll look up the full profile and history for that specific customer in Jumpseller.


## Installation & Usage

To install and use the **Jumpseller** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jumpseller](https://vinkius.com/mcp/jumpseller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
