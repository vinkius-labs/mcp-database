# Clover POS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clover-pos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clover-pos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clover-pos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Connect to your Clover merchant account — manage orders, inventory, customers, and payments directly via AI.

## Description
Integrate your AI agent with **Clover**, the leading point-of-sale (POS) system. This integration allows you to monitor your business operations in real-time, from tracking orders and managing inventory to inspecting customer data and payment history.

### What you can do

- **Order Monitoring** — List and retrieve detailed information for all merchant orders
- **Inventory Control** — Access your full catalog of items, categories, and organize stock data
- **Customer Oversight** — Lookup customer profiles and transaction histories
- **Merchant Intelligence** — Get basic settings, currency info, and physical address data for your business
- **Staff Management** — List employees and their assigned roles within the Clover ecosystem
- **Payment & Tax Auditing** — Review processed payments and configured sales tax rates

### How it works

1. Subscribe to this server
2. Enter your **Clover Access Token** and **Merchant ID** (mId)
3. Start managing your store operations through natural conversation

### Who is this for?

- **Business Owners** — quickly check daily orders and inventory levels without opening the Clover dashboard
- **Store Managers** — retrieve employee lists and customer data for operational tasks
- **Accountants** — audit payment logs and tax rates via AI assistance


## Available Tools
- **get_merchant_info**: Retrieve basic information about the Clover merchant
- **get_order_details**: Retrieve detailed information for a specific order
- **list_inventory_categories**: List inventory categories
- **list_customers**: Retrieve a list of customers associated with the merchant
- **list_device_access_tokens**: List access tokens associated with merchant devices
- **list_employees**: Retrieve a list of merchant employees
- **list_inventory_items**: List all items in the merchant inventory
- **list_orders**: Retrieve a list of orders for the merchant
- **list_payments**: Retrieve a list of processed payments
- **list_tax_rates**: Retrieve sales tax rates configured for the merchant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clover POS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all orders from my Clover store."

**🤖 AI Agent:**
> Fetching orders... I found several recent orders, including #ORD-123 ($45.00, Paid) and #ORD-124 ($12.50, Open). Would you like the details for a specific order?

---

**👤 You:**
> "Check inventory items."

**🤖 AI Agent:**
> Accessing inventory... Your catalog includes 'Organic Coffee' ($18.00), 'Green Tea' ($12.00), and 'Pastry Box' ($25.00).


## Installation & Usage

To install and use the **Clover POS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clover-pos](https://vinkius.com/mcp/clover-pos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
