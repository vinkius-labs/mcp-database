# Stripe Legacy MCP Server

Manage payments, customers, and account balances on Stripe via the legacy API with AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stripe-legacy)

## Overview
**Category:** industry-titans
**Tools Count:** 11

## Description
Connect your **Stripe** account to any AI agent to automate your basic payment processing and customer management. This integration provides a streamlined interface for the core Stripe v1 API, allowing you to monitor charges, create payment tokens, and track account balances through natural conversation.

### What you can do

- **Payment Orchestration** — List recent charges and retrieve detailed metadata for specific transactions programmatically.
- **Customer Management** — Access and monitor your customer database to keep your client records synchronized directly from the AI interface.
- **Charge Lifecycle Control** — Create new charges and manage payment tokens using simple AI commands to facilitate transactions.
- **Financial Monitoring** — Retrieve your real-time Stripe account balance to ensure your business liquidity is always visible.
- **Operational Oversight** — Get instant summaries of recent payment activity and customer metadata via natural language.

### How it works

1. Subscribe to this server
2. Enter your Stripe Secret Key (sk_...) from your dashboard
3. Start managing your payment operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Owners** — quickly check recent sales and account balances without switching apps.
- **Support Teams** — automate the retrieval of customer charge details to resolve billing inquiries via natural conversation.
- **Developers** — test core Stripe payment flows and monitor balances directly within the chat.


## Available Tools
- **create_charge**: Pass data as a JSON string.

Create a new charge
- **create_customer**: Create a new Stripe customer
- **create_refund**: Create a refund for a charge
- **create_token**: Pass data as a JSON string.

Create a single-use token
- **get_balance**: Check account balance
- **get_charge**: Get charge details
- **get_customer**: Get details for a specific customer
- **list_charges**: List all Stripe charges
- **list_customers**: List all Stripe customers
- **list_invoices**: List all invoices
- **list_subscriptions**: List all active subscriptions


## Installation & Usage

To install and use the **Stripe Legacy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stripe-legacy](https://vinkius.com/mcp/stripe-legacy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
