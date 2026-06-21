# Worldpay MCP Server

Process payments, manage refunds, and audit settlements on Worldpay — the global leader in payment processing technology.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/worldpay)

## Overview
**Category:** money-moves
**Tools Count:** 9

## Description
Connect your **Worldpay** account to any AI agent and manage your global payment operations through natural conversation.

### What you can do

- **Payment Processing** — Initiate new payment orders using secure tokens and retrieve real-time transaction statuses instantly
- **Refund Management** — Process partial or full refunds for previously completed payments directly from your agent
- **Tokenization** — Create and manage reusable payment tokens to securely store customer card data without handling raw sensitive information
- **Settlement Auditing** — List and monitor funds that have been settled to your account, including granular transaction-level breakdowns
- **Webhook Governance** — Verify the configuration of your real-time notification endpoints to ensure payment updates are being delivered
- **Operational Insights** — Quickly find unique order codes, token IDs, and settlement batches required for financial reconciliation
- **Connectivity Health** — Verify the operational status of your Worldpay API integration to ensure your payment gateway is always reachable

### How it works

1. Subscribe to this server
2. Enter your Worldpay Service Key
3. Start managing your payments and settlements through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex banking dashboards to verify a payment. Your AI agent becomes your payment operations coordinator.

### Who is this for?

- **Finance Teams** — monitor settlements and reconcile daily payment batches through simple chat commands
- **E-commerce Managers** — process customer refunds and verify order statuses without manual data entry
- **Developers** — test payment tokenization and verify webhook configurations through conversation
- **Customer Support** — quickly lookup transaction details and payment histories to provide rapid assistance


## Available Tools
- **create_payment_order**: Provide the payment token, amount, currency, and order description.

Creates a new payment order in Worldpay
- **create_reusable_token**: Generates a reusable payment token from sensitive card data
- **get_api_health**: Checks the operational status of the Worldpay API connection
- **get_order_details**: Retrieves details for a specific payment order
- **get_settlement_details**: Retrieves granular details for a specific settlement
- **get_token_details**: Retrieves metadata for a specific payment token
- **list_payment_settlements**: Lists funds that have been settled to your account
- **list_webhook_endpoints**: Lists all registered webhook notification endpoints
- **refund_payment_order**: Provide the order code and the amount to refund.

Refunds a previously completed payment


## Installation & Usage

To install and use the **Worldpay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/worldpay](https://vinkius.com/mcp/worldpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
