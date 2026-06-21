# Douyin Local Life API / 抖音生活服务 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/douyin-local-life-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/douyin-local-life-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/douyin-local-life-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's leading local life platform — manage shops, process orders, and verify coupons via AI.

## Description
Empower your AI agent to orchestrate your local retail and hospitality operations with **Douyin Local Life** (抖音生活服务), the dominant social commerce platform in China. By connecting Douyin to your agent, you transform complex shop management, order fulfillment, and coupon verification into a natural conversation. Your agent can instantly retrieve shop metadata, update product stock levels, verify customer coupons, and audit real-time order flows without you ever needing to navigate the comprehensive Douyin Merchant Center. Whether you are automating a busy restaurant or monitoring multiple retail branches, your agent acts as a real-time digital manager, providing accurate and fast results from a single, authorized source.

### What you can do

- **Shop Orchestration** — Retrieve shop info, search for nearby POIs, and monitor store status in real-time.
- **Order Management** — List recent orders, retrieve detailed metadata, and audit fulfillment progress.
- **Coupon Verification** — Retrieve and verify customer coupon codes to ensure secure and valid fulfillment.
- **Inventory Control** — Monitor and update product stock levels across specific POIs to prevent overbooking.
- **Product Discovery** — Access detailed product information and metadata for your life service offerings.

### How it works

1. Subscribe to this server
2. Enter your Douyin Client Key, Client Secret, and App Private Key
3. Start managing your local life operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant & Hotel Managers** — manage order lifecycles and coupon verifications through natural language queries.
- **Retail Operations** — monitor inventory levels and audit shop performance directly from your AI-powered workspace.
- **Developers** — integrate professional local life APIs into your AI-driven daily routines.
- **Douyin Power Users** — integrate your existing merchant workflows into your AI-driven daily routines.


## Available Tools
- **get_order_detail**: Get order details
- **get_product_detail**: Get product metadata
- **get_product_stock**: Get product inventory
- **get_shop_info**: Get shop metadata
- **get_verify_code**: Get order verification code
- **list_recent_orders**: List recent orders
- **search_shops**: Search for shops
- **update_product_stock**: Update product inventory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Douyin Local Life API / 抖音生活服务** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the details for shop with POI ID 'POI_88210934'."

**🤖 AI Agent:**
> I've retrieved the shop metadata. 'Tasty Dumplings' (ID: `POI_88210934`) is currently active and located in the Pudong District of Shanghai. Would you like me to check the current inventory levels for this shop?

---

**👤 You:**
> "Verify coupon code '12345678' for shop 'POI_8821'."

**🤖 AI Agent:**
> I've successfully verified the coupon code. It is valid for a 'Premium Set Menu'. The order has been marked as fulfilled in the Douyin system. Should I list any other pending orders for this shop?

---

**👤 You:**
> "What is the current stock for product 'PRD_9920' at shop 'POI_8821'?"

**🤖 AI Agent:**
> The current stock level for 'PRD_9920' at the specified shop is 45 units. Would you like me to update this stock or check the product's performance data?


## Installation & Usage

To install and use the **Douyin Local Life API / 抖音生活服务** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/douyin-local-life-api](https://vinkius.com/mcp/douyin-local-life-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
