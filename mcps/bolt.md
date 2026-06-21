# Bolt MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bolt)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bolt-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bolt-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage your one-click checkout and payments via Bolt — track transactions, manage orders, and process refunds directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bolt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 transactions in my Bolt account."

**🤖 AI Agent:**
> I've retrieved your recent transactions. Notable entries include a $45.00 charge (Ref: ABC-123) and a $120.00 authorization (Ref: XYZ-789). Would you like full details for any of them?

---

**👤 You:**
> "Refund $20.00 for transaction reference ABC-123."

**🤖 AI Agent:**
> I've initiated a partial refund of $20.00 (2000 cents) for transaction ABC-123. The credit process has started in your Bolt merchant account.

---

**👤 You:**
> "Check the status of my Bolt merchant account."

**🤖 AI Agent:**
> Your merchant account is currently 'Active' and all configurations are valid. Your publishable key ends in '...xyz' and your division ID is 'div_123'.


## Installation & Usage

To install and use the **Bolt** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bolt](https://vinkius.com/mcp/bolt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
