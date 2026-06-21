# Getpaid MCP Server

Manage billing, track payments, and initiate checkouts via AI agents with Getpaid.io.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/getpaid)

## Overview
**Category:** finance-accounting
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Getpaid** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getpaid](https://vinkius.com/mcp/getpaid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
