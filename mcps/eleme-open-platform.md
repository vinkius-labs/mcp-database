# Ele.me Open Platform / 饿了么 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eleme-open-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eleme-open-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eleme-open-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's massive food delivery API — manage shops, process orders, and track deliveries via AI.

## Description
Empower your AI agent to orchestrate your food delivery business with the **Ele.me Open Platform** (饿了么), one of the largest on-demand delivery networks in the world. By connecting Ele.me to your agent, you transform complex merchant operations, order fulfillment, and delivery tracking into a natural conversation. Your agent can instantly retrieve shop metadata, confirm incoming orders, manage product categories, and audit real-time delivery states without you ever needing to navigate the comprehensive Ele.me Merchant Center. Whether you are automating a busy kitchen or monitoring customer feedback across a retail chain, your agent acts as a real-time digital manager, providing accurate and fast results from a single, authorized source.

### What you can do

- **Shop Orchestration** — Retrieve shop info, open or close stores, and list product categories.
- **Order Management** — Confirm new orders, retrieve detailed metadata, and cancel orders with specific remarks.
- **Delivery Tracking** — Monitor the real-time state of the courier and the delivery progress for any order.
- **Feedback Auditing** — Retrieve and analyze user comments and ratings to maintain service quality.
- **Inventory Control** — Access and browse shop categories to coordinate menu availability.

### How it works

1. Subscribe to this server
2. Enter your Ele.me App Key, App Secret, and Access Token
3. Start managing your delivery business through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Restaurant Owners** — manage order workflows and shop status through natural language queries.
- **Retail Operations** — monitor delivery efficiency and audit merchant performance directly from your AI-powered workspace.
- **Developers** — integrate professional food delivery APIs into your AI-driven daily routines.
- **Ele.me Power Users** — integrate your existing merchant workflows into your AI-driven daily routines.


## Available Tools
- **cancel_order**: Cancel an order
- **close_shop**: Set shop status to closed
- **confirm_order**: Confirm an order
- **get_order_comments**: Get order comments
- **get_order_detail**: Get order details
- **get_shop_info**: Get shop metadata
- **list_recent_orders**: List recent orders
- **list_shop_categories**: List shop product categories
- **open_shop**: Set shop status to open
- **track_delivery**: Track delivery state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ele.me Open Platform / 饿了么** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the metadata for shop 'SHOP_88210934'."

**🤖 AI Agent:**
> I've retrieved the shop metadata. 'Happy Noodles' (ID: `SHOP_88210934`) is currently 'Open' and has a 4.8-star rating. It is located at '123 Main St, Shanghai'. Would you like to see the available product categories for this shop?

---

**👤 You:**
> "List the most recent orders for my shop."

**🤖 AI Agent:**
> I've retrieved your recent orders. You have 5 new orders waiting for confirmation. The most recent is `ORD_9920` for 85.00 CNY. Should I provide the detailed item breakdown for this order?

---

**👤 You:**
> "Track the delivery state for order 'ORD_8821'."

**🤖 AI Agent:**
> The delivery state for order `ORD_8821` is currently 'In Transit'. The courier, 'Li Qiang', is on his way to the customer. He was last located 500 meters from the destination. I'll monitor for the 'Delivered' confirmation.


## Installation & Usage

To install and use the **Ele.me Open Platform / 饿了么** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eleme-open-platform](https://vinkius.com/mcp/eleme-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
