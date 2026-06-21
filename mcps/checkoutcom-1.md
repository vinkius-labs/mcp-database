# Checkout.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkoutcom-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/checkoutcom-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/checkoutcom-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage global payments via Checkout.com — process payments, capture funds, handle refunds, and vault instruments directly from any AI agent.

## Description
Connect your **Checkout.com** account to any AI agent and take full control of your payment workflows through natural conversation.

### What you can do

- **Payments** — Request, capture, void, and refund payments with support for various currencies and sources
- **Vaulting (Instruments)** — Securely create, list, update, and delete payment instruments (cards) in the Checkout.com Vault
- **Payment Actions** — Track every action taken on a payment to understand authorization successes and failures
- **Analytics & History** — Audit payment statuses and details directly from your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkout.com Secret API Key and choose your environment (Sandbox or Live)
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce teams** — handle refunds and voids without jumping between tabs or specialized dashboard views
- **Developers** — test payment flows in sandbox using natural language or debug instrument vaulting logic
- **Finance teams** — audit payment actions and verify capture statuses for reconciliation
- **Customer support** — look up payment details and history to resolve billing inquiries faster


## Available Tools
- **capture_payment**: /captures` locking an authorized transaction converting it to native settled limits.

Retrieve the exact structural matching verifying Capture processing
- **create_instrument**: Provision a highly-available JSON Payload generating hard Customer bindings
- **delete_instrument**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **get_payment_actions**: Enumerate explicitly attached structured rules exporting Gateway state
- **get_instrument**: Identify precise active arrays spanning native Vault logic
- **get_payment_details**: com nodes.

Perform structural extraction of properties driving active Billing logic
- **refund_payment**: /refunds` moving hard cash back exactly to the originating Visa/MC network.

Dispatch an automated validation check routing explicit Clawback logic
- **request_payment**: Identify bounded CRM records inside the Headless Checkout.com Gateway
- **update_instrument**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **void_payment**: /voids` dropping limits before a capture closes cutting out heavy gateway fees.

Inspect deep internal arrays mitigating specific Plan Math


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkout.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Refund payment pay_123 for $50.00"

**🤖 AI Agent:**
> Refund request sent for pay_123. The refund of $50.00 (5000 minor units) has been successfully initiated at the gateway.

---

**👤 You:**
> "Show me why payment pay_456 failed"

**🤖 AI Agent:**
> Analyzing payment actions for pay_456... The authorization was declined with code '20059' (Insufficient Funds). The bank blocked the capture during the final settlement step.

---

**👤 You:**
> "Vault this instrument ID src_789 and update the holder name to 'John Doe'"

**🤖 AI Agent:**
> Instrument src_789 has been updated in the Vault. The holder name is now set to 'John Doe'. You can now use this instrument for future payment requests.


## Installation & Usage

To install and use the **Checkout.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkoutcom-1](https://vinkius.com/mcp/checkoutcom-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
