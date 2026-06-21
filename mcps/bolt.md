# Bolt MCP Server

Manage your one-click checkout and payments via Bolt — track transactions, manage orders, and process refunds directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bolt)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your **Bolt Merchant** account to any AI agent and orchestrate your checkout and payment workflows through natural conversation.

### What you can do

- **Transaction Oversight** — List recent Bolt transactions and retrieve detailed metadata for individual payments.
- **Payment Lifecycle Management** — Capture authorized transactions, void pending ones, and issue full or partial refunds.
- **Order Token Generation** — Create order tokens to initiate secure one-click checkout sessions.
- **Shopper Intelligence** — Retrieve account details and order history for authenticated shoppers.
- **Webhook Monitoring** — List and audit configured webhooks to ensure real-time data sync.
- **Merchant Health Check** — Retrieve the current status and configuration of your merchant account.

### How it works

1. Subscribe to this server
2. Enter your Bolt Private API Key and Environment (api or api-sandbox)
3. Start managing your checkout experience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Operations** — quickly check payment statuses and process refunds without manual dashboard work.
- **Customer Support** — retrieve transaction details and order history straight from their workflow tools.
- **Developers** — verify API integrations and order token generation using natural language.


## Available Tools
- **capture_transaction**: Capture a previously authorized transaction
- **create_order_token**: Create an order token to initiate checkout
- **get_account_details**: Get current account details
- **get_merchant_status**: Check the current merchant account status
- **get_order_details**: Get details of a specific order
- **get_transaction**: Get details of a specific transaction
- **list_transactions**: List recent Bolt transactions
- **list_webhooks**: List configured webhooks
- **refund_transaction**: Issue a refund for a completed transaction
- **void_transaction**: Void an authorized but uncaptured transaction


## Installation & Usage

To install and use the **Bolt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bolt](https://vinkius.com/mcp/bolt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
