# Checkout.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkoutcom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkoutcom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkoutcom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage global payments via Checkout.com — track transactions, process refunds, and monitor account health directly from any AI agent.

## Description
Connect your **Checkout.com** account to any AI agent and take full control of your global payment operations through natural conversation. Streamline how you manage transactions across 150+ currencies.

### What you can do

- **Unified Payment Oversight** — List and retrieve details for all payments processed through the Unified API natively
- **Mutable Operations** — Refund, capture, or void payments directly through secure conversational commands flawlessly
- **Action Auditing** — List all lifecycle actions for any specific payment to track its history securely
- **Connectivity Monitoring** — List and review configured webhooks to ensure your integration is running flawlessly
- **System Metadata** — Retrieve core account information and user settings directly within your workspace flawlessly
- **minor unit Handling** — Work with precise financial amounts in minor units for high-accuracy transaction management

### How it works

1. Subscribe to this server
2. Enter your Checkout.com Secret Key and API Prefix
3. Start managing your global payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — monitor transaction volumes and process refunds using natural language
- **E-commerce Managers** — audit payment statuses and lifecycle actions without opening the hub
- **Customer Support** — quickly verify payment results and capture authorizations straight from their chat interface
- **Developers** — verify webhook delivery and API connectivity during technical implementation


## Available Tools
- **capture_checkout_payment**: Capture an authorized payment
- **get_checkout_account_info**: Retrieve core account and user information
- **list_payment_actions**: List all lifecycle actions for a specific payment
- **get_payment_details**: Get detailed information for a specific payment
- **list_checkout_payments**: List recent payments
- **list_checkout_webhooks**: List configured webhooks
- **refund_checkout_payment**: Refund a captured payment
- **void_checkout_payment**: Void an authorized payment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkout.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my last 5 payments in Checkout.com."

**🤖 AI Agent:**
> Retrieving your recent payments... I found 5 items: Order #ABC ($120.00 - Captured), #DEF ($45.50 - Authorized), and 3 others. Would you like to see the actions history for any of these?

---

**👤 You:**
> "What happened to payment ID 'pay_123456'?"

**🤖 AI Agent:**
> Checking payment pay_123456... This payment was Authorized at 10:30 AM, then Captured at 10:35 AM for $99.00. No further actions have been recorded.

---

**👤 You:**
> "Refund payment pay_789 for $10.50."

**🤖 AI Agent:**
> Processing refund of $10.50 (1050 minor units) for pay_789... The refund has been successfully requested. The new status will be reflected in the payment actions shortly.


## Installation & Usage

To install and use the **Checkout.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkoutcom](https://vinkius.com/mcp/checkoutcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
