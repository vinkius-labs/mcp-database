# Getpaid MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getpaid)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/getpaid-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/getpaid-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage billing, track payments, and initiate checkouts via AI agents with Getpaid.io.

## Description
Connect your **Getpaid** account to any AI agent to automate your billing, payment processing, and checkout workflows through the Model Context Protocol (MCP). Getpaid is a modern payment platform designed for SaaS, marketplaces, and service businesses to handle global transactions with ease. This MCP server enables you to track payments, manage customer records, and initiate new checkout sessions directly through natural conversation.

### Key Features

- **Payment Oversight** — List all processed payments, fetch detailed metadata including status and timestamps, and monitor revenue flow instantly.
- **Checkout Automation** — Create new checkout sessions for products or services and retrieve secure payment links programmatically.
- **Refund Management** — Process full or partial refunds for captured payments directly from your chat interface.
- **Customer & Invoice Tracking** — Access your billing database, retrieve detailed customer profiles, and monitor generated invoices.
- **Subscription Insights** — List active and inactive recurring billing plans to understand your long-term revenue health.
- **Webhook Visibility** — Monitor configured webhooks to ensure your internal systems are receiving real-time payment notifications.
- **Real-time Synchronization** — Keep your financial operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Getpaid Client ID and Client Secret (found in your Integration Settings)
3. Start managing your billing and payments from Claude, Cursor, or any MCP client

### Who is this for?

- **Finance & Ops Managers** — quickly check payment statuses or process a refund without manual dashboard navigation.
- **Customer Support** — verify if a customer's payment was successful or retrieve invoice details via simple AI commands.
- **SaaS Founders** — get a real-time overview of active subscriptions and recent checkout sessions.


## Available Tools
- **verify_api_connection**: Check connection
- **create_checkout_session**: Initiate checkout
- **get_account_details**: Get account identity
- **get_checkout_status**: Check checkout status
- **get_customer_details**: Get customer metadata
- **get_payment_details**: Get payment metadata
- **list_billing_customers**: List customers
- **list_billing_invoices**: List invoices
- **list_billing_payments**: List all payments
- **list_billing_subscriptions**: List recurring plans
- **list_payment_webhooks**: List webhook configs
- **refund_billing_payment**: Process a refund


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Getpaid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all payments processed today."

**🤖 AI Agent:**
> Retrieving payments... I found 5 payments processed today, including a $50.00 charge (Status: Captured) and a $15.00 charge. Would you like the full details for any of them?

---

**👤 You:**
> "Create a checkout session for $25.00 USD."

**🤖 AI Agent:**
> Checkout initiated! I've successfully created a session for 2500 cents ($25.00 USD). The Checkout ID is 'chk_abc123'. You can share this link with the customer: [Payment Link].

---

**👤 You:**
> "Refund payment 'pay_98765' for the full amount."

**🤖 AI Agent:**
> Refund processed! I have successfully initiated a full refund for payment pay_98765. The status is now 'refunded' and the customer will see the credit shortly.


## Installation & Usage

To install and use the **Getpaid** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getpaid](https://vinkius.com/mcp/getpaid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
