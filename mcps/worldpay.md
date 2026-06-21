# Worldpay MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/worldpay)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/worldpay-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/worldpay-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Process payments, manage refunds, and audit settlements on Worldpay — the global leader in payment processing technology.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Worldpay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a payment order for 50.00 GBP using token 'tok-123'."

**🤖 AI Agent:**
> I've initiated the payment order for 50.00 GBP (5000 minor units) via Worldpay. Transaction successful! Your order code is 'ORD-XYZ-789'. Would you like me to pull the full receipt details?

---

**👤 You:**
> "Refund 20.00 USD for order 'ORD-ABC-456'."

**🤖 AI Agent:**
> Success! I've processed a refund of 20.00 USD (2000 minor units) for order ORD-ABC-456. The status has been updated in Worldpay and the customer will receive the funds according to their bank's policy.

---

**👤 You:**
> "Show me my latest account settlements."

**🤖 AI Agent:**
> I found 3 recent settlements: 1. ID: set-101 (Amount: 1,250.50 GBP, Date: 2026-03-28), 2. ID: set-102 (Amount: 890.00 GBP, Date: 2026-03-25), and 3. ID: set-103 (Amount: 2,100.00 GBP, Date: 2026-03-22). Which batch would you like to reconcile?


## Installation & Usage

To install and use the **Worldpay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/worldpay](https://vinkius.com/mcp/worldpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
