# ManoMano (Home Improvement Marketplace) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/manomano-home-improvement-marketplace)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/manomano-home-improvement-marketplace-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/manomano-home-improvement-marketplace-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Manage your ManoMano seller account — update offer prices, track orders, and audit fulfillment stock.

## Description
Connect your **ManoMano Seller** account to any AI agent and take full control of your marketplace operations and home improvement catalog through natural conversation.

### What you can do

- **Offer Orchestration** — List all published offers and retrieve detailed metadata including current stock, VAT-included pricing, and SKUs directly from your agent
- **Live Catalog Updates** — Safely modify VAT-included prices and update available inventory quantities for specific offers to maintain competitive market positioning
- **Order Management** — List all received orders and retrieve complete representations including customer details, delivery addresses, and individual line items securely
- **Logistical Control** — Acknowledge and accept pending orders or transition them to 'Shipped' status by supplying carrier-specific tracking numbers and carrier names
- **Fulfillment Visibility** — Monitor stock levels maintained through ManoFulfillment (ManoMano warehouse) to ensure logistical accuracy and product availability
- **Taxonomy Discovery** — Enumerate root category lists and registered brands to guide product mapping and architectural catalog taxonomy natively

### How it works

1. Subscribe to this server
2. Enter your ManoMano API Key
3. Start managing your marketplace presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketplace Sellers** — manage pricing and stock levels through natural conversation without manual Seller Central exports
- **E-commerce Managers** — monitor order flow and retrieve customer delivery data directly from your workspace for rapid auditing
- **Logistics Teams** — update shipping statuses and audit ManoFulfillment stock levels efficiently to maintain high fulfillment standards


## Available Tools
- **list_offers**: List all published offers on ManoMano
- **get_offer**: Get details for a specific ManoMano offer (price, stock, SKU)
- **update_offer_price**: This is a reversible operation.

Change the price of a specific offer
- **update_offer_stock**: This is a reversible operation.

Update the available stock count for a specific offer
- **list_orders**: List all received ManoMano orders
- **get_order**: Get full order details including customer, addresses, and order lines
- **accept_order**: Accept a pending ManoMano order
- **ship_order**: Ship an order by supplying a valid tracking number and carrier
- **list_categories**: List ManoMano catalog categories
- **list_brands**: List available brands on ManoMano
- **list_fulfillment_stock**: Check stock maintained through ManoFulfillment (ManoMano warehouse)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ManoMano (Home Improvement Marketplace)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all ManoMano orders received today"

**🤖 AI Agent:**
> I've retrieved 5 new orders. Highlights include Order #MM-123 (Amount: €45.00, Status: Pending) and Order #MM-456 (Amount: €120.00, Status: Accepted). Would you like to see the delivery address for the pending order?

---

**👤 You:**
> "Update the stock for offer 'offer-987' to 50 units"

**🤖 AI Agent:**
> Updating inventory… I've successfully set the stock for offer 'offer-987' to 50 units. Your listing on ManoMano is now synchronized with this new quantity. Would you like me to check the current price as well?

---

**👤 You:**
> "Show me the stock levels in ManoFulfillment"

**🤖 AI Agent:**
> Retrieving fulfillment stock… I've identified several items in the ManoMano managed warehouse. You have 150 units of SKU 'DRILL-01' and 45 units of SKU 'SAW-05'. No low-stock alerts detected for today.


## Installation & Usage

To install and use the **ManoMano (Home Improvement Marketplace)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/manomano-home-improvement-marketplace](https://vinkius.com/mcp/manomano-home-improvement-marketplace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
