# Dola Checkout MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dola-checkout)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dola-checkout-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dola-checkout-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Accept payments globally with a checkout experience designed for digital products, subscriptions, and one-time purchases.

## Description
Connect your **Dola Checkout** account to any AI agent and take full control of your e-commerce transaction and shopper engagement workflows through natural conversation.

### What you can do

- **Order Orchestration** — List and manage all online store orders programmatically, including monitoring payment status and fulfillment in real-time
- **Session Architecture** — Programmatically create new checkout sessions and generate secure payment URLs for your customers to streamline the buying process
- **Shopper Intelligence** — Access complete shopper profiles and monitor their purchase history to maintain high-fidelity customer relationship records
- **Connectivity Monitoring** — Configure and manage real-time data sync webhooks directly through your agent for reliable transaction processing
- **Merchant Visibility** — Access high-level merchant account metadata and sales summaries directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Secret API Key** from your Dola dashboard (Settings > API)
3. Start managing your 1-click checkout transactions from Claude, Cursor, or any MCP client

No more manual order searching or complex checkout URL generation in the dashboard. Your AI acts as your dedicated e-commerce operations and payment coordinator.

### Who is this for?

- **E-commerce Merchants** — instantly retrieve order details and check shopper history using natural language commands
- **Marketing & Growth Teams** — generate checkout URLs for specific products or campaigns without leaving your workspace
- **Developers & Ops** — automate transaction monitoring and manage webhook configurations through simple AI queries


## Available Tools
- **create_checkout**: Create a checkout session
- **create_order**: Create a new order
- **create_webhook**: created.

Create a new webhook
- **get_account_info**: Get account profile
- **get_checkout**: Get checkout details
- **get_customer**: Get customer details
- **get_order**: Get order details
- **list_checkouts**: List active checkouts
- **list_customers**: List all customers
- **list_orders**: List all checkout orders
- **list_webhooks**: List active webhooks
- **update_order**: Update order status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dola Checkout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active checkout orders in my Dola account."

**🤖 AI Agent:**
> I've retrieved your recent orders. You currently have 5 active transactions, including Order #4502 (Completed) and #4503 (Pending). Would you like the shopper details for any of these?

---

**👤 You:**
> "Create a checkout session for a 'MacBook Pro' priced at $1999.00."

**🤖 AI Agent:**
> Checkout session generated! I've created a new session for the MacBook Pro. You can share this secure URL with the customer: [checkout_url]. The session ID is 'sess_123'.

---

**👤 You:**
> "Show the purchase history for shopper ID 'cust_789'."

**🤖 AI Agent:**
> Fetching history... Shopper cust_789 has made 3 past purchases totaling $2,450. Notable orders include a 'Workstation' and 'Monitor Stand'. Shall I check the fulfillment status for their latest order?


## Installation & Usage

To install and use the **Dola Checkout** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dola-checkout](https://vinkius.com/mcp/dola-checkout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
