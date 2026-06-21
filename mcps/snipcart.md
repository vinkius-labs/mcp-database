# Snipcart MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snipcart)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snipcart-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snipcart-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your headless e-commerce store to your AI. List orders, update fulfillment statuses, and manage customers seamlessly from your environment.

## Description
Connect your **Snipcart** merchant dashboard with your favorite AI agent. Control your headless shopping cart backend seamlessly through natural language in your code editor. Rather than switching contexts to manage products and monitor checkouts, handle your entire back office autonomously via MCP.

### What you can do

- **Order Fulfillment** — Extract newly processed purchases calling `list_orders` and actively change shipping phases using `update_order_status`
- **Customer CRM** — Survey buyer behavior natively by pulling data securely with `list_customers` and inspecting individuals via `get_customer_details`
- **Catalog & Subscriptions** — Monitor active inventory logic calling `list_products` or manage recurring rebilling schedules via `list_subscriptions`
- **Marketing Intel** — Keep track of promotional coupons and sales campaigns directly using `list_discounts`

### How it works

1. Subscribe to this server
2. Supply your Snipcart Secret API Key (Live or Test environments)
3. Prompt Claude, Cursor, or Windsurf to read your cart metrics

Stop digging through dashboard menus to figure out if your discount script is working. Validate product availability and user checkout status directly where your code lives.

### Who is this for?

- **E-Commerce Founders** — instantly ask for specific order statuses without opening a single web browser window
- **Full-Stack Developers** — test 'Live' or 'Test' mode transactions reliably when building new headless storefronts (Next.js, Nuxt)
- **Support Teams** — give the bot a customer’s email and have it retrieve the total order history immediately


## Available Tools
- **get_customer_details**: Retrieves details for a specific customer
- **get_order_details**: Retrieves details for a specific order
- **get_subscription_details**: Retrieves details for a specific subscription
- **list_customers**: Lists all registered customers
- **list_discounts**: Lists all active discount codes and promotions
- **list_orders**: Lists all e-commerce orders in Snipcart
- **list_products**: Lists all products configured in Snipcart
- **list_subscriptions**: Lists all active and inactive subscriptions
- **update_order_status**: g., "Processed", "Shipped").

Updates the status of an existing order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snipcart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find out what product was sold in our most recent completed order."

**🤖 AI Agent:**
> Scanning your orders using `list_orders`... 🔍

The last order (Token: `SNIP-9923`) belongs to Alice Smith.
**Items Bought**:
- 1x 'Stark Industries T-Shirt' (Price: $29.99)
- 2x 'Enamel Logo Pin' (Price: $10.00 each)

**Total Transaction**: $49.99 (Paid & Processed).

---

**👤 You:**
> "I need to mark invoice SNIP-8910 as Shipped, please update the order status."

**🤖 AI Agent:**
> Status change request triggered via the `update_order_status` action hook. 

✅ Invoice **SNIP-8910** has been successfully transitioned to the **Shipped** state. E-mail triggers from your backend should process automatically to the buyer.

---

**👤 You:**
> "Output a markdown list of all active products and their prices we are offering on Snipcart."

**🤖 AI Agent:**
> Based on my scan of `list_products`, here is your current live inventory:

- **Space Rocket Figurine** - $45.00 (`id: spc-rckt`)
- **Moon Boots Replika** - $115.00 (`id: mn-bts-rep`)
- **Galactic Coffee Mug** - $22.50 (`id: glc-co-mug`) 

Inventory checks indicate no products are currently marked as out of stock.


## Installation & Usage

To install and use the **Snipcart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snipcart](https://vinkius.com/mcp/snipcart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
