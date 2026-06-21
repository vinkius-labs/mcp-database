# Paddle MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paddle)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/paddle-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/paddle-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage billing, subscriptions, and transactions via Paddle — inspect customers, list products, pause recurring plans, and void transactions from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paddle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the subscription details for sub_01h9z2..."

**🤖 AI Agent:**
> Subscription sub_01h9z2... is currently Active. Next billing date is set for Nov 14th, 2026. Billed at $49/month (Pro SaaS Tier). It is tied to customer ctm_01jh1. Want me to pause it?

---

**👤 You:**
> "List our most recent revenue transactions on Paddle."

**🤖 AI Agent:**
> I extracted the latest transactions from Paddle Billing. 1. txn_1w2... (Paid: $19.00 USD). 2. txn_4x9... (Prorated: $10.50 USD). 3. txn_9z2... (Paid: $99.00 USD). Want me to pull specific tax boundaries applied on the $99 payment?

---

**👤 You:**
> "Cancel subscription sub_active123 at the end of the billing cycle."

**🤖 AI Agent:**
> Action complete. Subscription sub_active123 has been marked for cancellation effective mapping `next_billing_period`. The user will not be charged again by the MoR, but remains active until the pre-paid term expires.


## Installation & Usage

To install and use the **Paddle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paddle](https://vinkius.com/mcp/paddle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
