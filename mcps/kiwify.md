# Kiwify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kiwify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kiwify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kiwify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Sell digital products and online courses in the Brazilian market with a platform that handles payments, delivery, and affiliates.

## Description
Connect your **Kiwify** account to any AI agent and manage digital product sales through natural conversation.

### What you can do

- **Product Management** — List products, inspect details, and track sales performance
- **Order Tracking** — Browse orders with status, amounts, and customer data
- **Subscription Monitoring** — Track active subscriptions, renewals, and churn
- **Customer Database** — List customers with purchase history and engagement
- **Revenue Analytics** — Monitor sales metrics, refund rates, and trends

### How it works

1. Subscribe to this server
2. Enter your Kiwify Access Token and Account ID
3. Start managing sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Creators** — track product sales and customer data
- **Info-product Entrepreneurs** — monitor subscriptions and revenue
- **Marketing Teams** — analyze sales performance and conversion metrics


## Available Tools
- **create_notification_webhook**: Create a new webhook
- **delete_notification_webhook**: Remove an existing webhook
- **get_account_summary**: Get account information
- **get_product_details**: Get details for a specific product
- **get_sale_details**: Get details for a specific sale
- **list_products**: List your Kiwify products
- **list_sales_history**: Supports filtering.

List recent sales and transactions
- **list_active_subscriptions**: List recurring subscriptions
- **list_configured_webhooks**: List your webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kiwify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all products with sales performance and today's orders."

**🤖 AI Agent:**
> Products: 5. 'Marketing Digital Pro' (R$497, 1.2K sales, R$596K total). 'SEO Masterclass' (R$297, 890 sales, R$264K). 'Social Media Kit' (R$97, 2.1K sales, R$204K). Today: 8 orders. 3 'Marketing Digital Pro', 2 'SEO', 3 'Social Media'. Revenue today: R$2,582. Refunds: 0.

---

**👤 You:**
> "Show active subscriptions and churn rate for this month."

**🤖 AI Agent:**
> Active subscriptions: 342. 'Marketing Digital Pro Monthly' (180, R$97/mo). 'SEO Membership' (120, R$67/mo). 'All Access' (42, R$197/mo). MRR: R$33,054. This month: +28 new, -12 cancelled. Churn rate: 3.5% (industry avg: 5-7%). Upcoming renewals: 45 in next 7 days.

---

**👤 You:**
> "Show the customer database and top buyers."

**🤖 AI Agent:**
> Customers: 4,190 total. This month: +248 new. Top by lifetime value: 1) João Silva — R$2,388 (All Access + courses). 2) Maria Santos — R$1,594 (3 products). 3) Carlos Mendes — R$1,291 (2 products + subscription). Average LTV: R$253. Repeat buyers: 18%.


## Installation & Usage

To install and use the **Kiwify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kiwify](https://vinkius.com/mcp/kiwify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
