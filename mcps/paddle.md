# Paddle MCP Server

Manage billing, subscriptions, and transactions via Paddle — inspect customers, list products, pause recurring plans, and void transactions from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/paddle)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Bring the **Paddle Billing API** directly into your AI workflows. Acting as your Merchant of Record (MoR) interface, this integration allows your agent to seamlessly query customer billing states, manage SaaS subscriptions, retrieve invoice ledgers, and pause actively churning plans natively.

### What you can do

- **Customers & Billing Details** — List and search all CRM accounts managed by Paddle and extract their exact tax identification boundaries
- **Subscription Lifecycle** — Inspect active or past-due subscriptions, cancel recurring flows dynamically, or pause an active schedule right from chat
- **Transactions & Ledgering** — Fetch bulk atomic transactions matching exact one-off payments, prorations, and historical subscription renewals
- **Catalog Explorer** — List your products and retrieve localized checkout prices and native tax-inclusive pricing definitions

### How it works

1. Subscribe to this server
2. Enter your Paddle API Key
3. Start managing active SaaS billing states from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support teams** — check payment status or pause subscriptions securely without requesting access to the Paddle dashboard
- **RevOps & Finance** — extract dynamic revenue limits, evaluate native transactional tax boundaries, and pull structured ledger arrays
- **SaaS Developers** — test billing configurations and checkout limits directly during product lifecycle testing


## Available Tools
- **cancel_subscription**: Can be set to effective immediately or at the end of the current billing period.

Cancel an active subscription
- **get_customer_details**: Get details for a specific customer
- **get_subscription_details**: Get details for a specific subscription
- **get_transaction_details**: Get details for a specific transaction
- **list_customers**: List all customers in Paddle
- **list_catalog_prices**: List all pricing definitions
- **list_catalog_products**: List all products
- **list_subscriptions**: List all subscriptions
- **list_transactions**: List all billing transactions
- **pause_subscription**: Pause an active subscription


## Installation & Usage

To install and use the **Paddle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paddle](https://vinkius.com/mcp/paddle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
