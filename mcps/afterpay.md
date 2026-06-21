# Afterpay MCP Server

Buy Now, Pay Later orchestration — manage checkouts, payments, and refunds via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/afterpay)

## Overview
**Category:** money-moves
**Tools Count:** 5

## Description
Connect your **Afterpay (Clearpay)** merchant account to your AI agent to unlock enterprise-grade BNPL (Buy Now, Pay Later) orchestration. From creating secure checkout tokens to monitoring payment statuses and processing partial refunds, your agent handles your financial transactions through natural conversation.

### What you can do

- **Checkout Orchestration** — Create new checkout sessions and retrieve secure redirect tokens for your customers
- **Payment Monitoring** — List and audit historical payments, check capture statuses, and retrieve technical metadata
- **Refund Management** — Initiate full or partial refunds for specific orders directly from your chat interface
- **Configuration Audit** — Retrieve merchant-specific configuration including minimum and maximum order limits
- **Transaction Insights** — Quickly identify successful captures or pending authorizations without manual dashboard exports

### How it works

1. Subscribe to this server
2. Enter your Afterpay Merchant ID and Secret Key
3. Start managing your BNPL transactions and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Operations** — automate refund processing and audit transaction logs effortlessly
- **E-commerce Managers** — monitor checkout health and verify order limit configurations on the fly
- **Customer Support Teams** — quickly look up payment statuses and order history to resolve billing inquiries
- **Developers** — verify API integration and inspect payment responses using simple commands


## Available Tools
- **get_afterpay_config**: Retrieve the minimum and maximum order transaction limits enforced by your Afterpay merchant account
- **create_checkout**: The amount must fall within the configured limits.

Initiate a secure Afterpay BNPL payment session token for a customer transaction
- **list_payments**: Retrieve historical BNPL transactions and authorizations securely from your Afterpay account
- **get_payment_details**: Retrieve detailed financial status, settlement info, and logs for a specific Afterpay order ID
- **refund_payment**: Always verify the remaining balance before refunding.

Initiate a full or partial refund to immediately credit a consumer against a previously captured Afterpay order


## Installation & Usage

To install and use the **Afterpay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/afterpay](https://vinkius.com/mcp/afterpay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
