# Mercado Libre MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mercado-libre)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mercado-libre-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mercado-libre-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Mercado Libre business via AI — list products, track orders, handle shipments, and answer buyer questions directly.

## Description
Connect your **Mercado Libre** seller account to any AI agent to streamline your e-commerce operations through natural conversation.

### What you can do

- **Product Listing** — Predict the correct category for your items and create new listings with full attribute support
- **Order Management** — Search and retrieve detailed metadata for orders, including status, payment, and buyer info
- **Logistics & Shipping** — Track shipment status and monitor SLA dispatch times to protect your seller reputation
- **Customer Service** — Search for buyer questions, provide answers, and manage post-sale messaging flows
- **Claims & Returns** — Inspect active claims and return details to resolve customer issues efficiently
- **Price & Promos** — Check sale prices and identify items eligible for promotions

### How it works

1. Subscribe to this server
2. Enter your Mercado Libre Access Token
3. Start managing your store from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — monitor store performance and order statuses without manual dashboard navigation
- **Support Teams** — respond to buyer questions and handle post-sale claims directly through the AI interface
- **Logistics Coordinators** — keep track of shipment deadlines and SLA compliance in real-time


## Available Tools
- **answer_question**: Answer a buyer question
- **create_item**: Requires title, category_id, price, currency_id, available_quantity, buying_mode, condition, listing_type_id, and pictures.

Publish a new item on Mercado Libre
- **create_test_user**: Create a test user
- **get_claim**: Get details of a post-purchase claim
- **get_me**: Get current Mercado Libre user info
- **get_order**: Get details for a specific order
- **get_post_sale_messages**: Get post-sale messages
- **get_promotion_candidate**: Check promotion eligibility
- **get_return_details**: Get details of a product return
- **get_sale_price**: Get the current sale price of an item
- **get_shipment_sla**: Get shipment SLA (Service Level Agreement)
- **get_shipment**: Get shipment information
- **get_user_addresses**: Get addresses for a specific user
- **predict_category**: Predict category for a product title
- **search_orders**: Search orders for a seller
- **search_questions**: Search questions for a seller
- **send_post_sale_message**: Send a post-sale message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mercado Libre** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all 'paid' orders for seller ID 123456789."

**🤖 AI Agent:**
> I've found 3 paid orders for seller 123456789. The most recent is order #2000001234 for a 'Smartphone XYZ'. Would you like to see the shipment details for this order?

---

**👤 You:**
> "What is the shipping status and SLA for shipment 405928374?"

**🤖 AI Agent:**
> Shipment 405928374 is currently 'ready_to_ship'. According to the SLA data, you must dispatch this item by tomorrow at 4:00 PM to maintain your reputation metrics.

---

**👤 You:**
> "Predict the best category for a 'Wireless Mechanical Keyboard' on site MLB."

**🤖 AI Agent:**
> For 'Wireless Mechanical Keyboard' on MLB (Brazil), the predicted category is MLB271505 (Keyboards). This category has a high probability match for your product title.


## Installation & Usage

To install and use the **Mercado Libre** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mercado-libre](https://vinkius.com/mcp/mercado-libre)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
