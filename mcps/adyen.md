# Adyen MCP Server

Global payment processing — manage payments, refunds, and merchant accounts via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/adyen)

## Overview
**Category:** money-moves
**Tools Count:** 4

## Description
Connect your **Adyen** account to your AI agent to unlock enterprise-grade payment orchestration and financial management. From monitoring real-time transaction statuses to handling refunds and auditing merchant account configurations, your agent handles your global payment ecosystem through natural conversation.

### What you can do

- **Payment Monitoring** — List and retrieve details for authorized, captured, or refused payments across your accounts
- **Refund & Modification** — Initiate refunds and manage payment modifications (captures, cancels) directly from chat
- **Merchant Oversight** — List and audit your merchant accounts and their technical configurations via the Management API
- **Payment Method Auditing** — Retrieve and verify available payment methods for specific regions and currencies
- **Financial Insights** — Quickly identify transaction trends and reconciliation patterns directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Adyen API Key and Merchant Account ID
3. Start managing your global payments and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Operations** — automate refund processing and payment status audits effortlessly
- **E-commerce Managers** — monitor checkout health and verify payment method availability on the fly
- **Customer Support** — check payment details and transaction history to resolve billing inquiries quickly
- **Developers** — verify API integration and inspect payment responses using simple commands


## Available Tools
- **get_payment_details**: Requires the 16-digit PSP reference.

Retrieve the full technical authorization and capture metadata for a specific Adyen payment
- **refund_payment**: Always double-check the amount before processing. Requires original PSP reference.

Initiate a full or partial refund for a previously captured payment in Adyen
- **list_merchants**: g. US, EU regions) and find a required Merchant ID.

Retrieve all active merchant accounts associated with your Adyen company profile
- **get_merchant_details**: Retrieve the technical configuration and status for a specific Adyen merchant account


## Installation & Usage

To install and use the **Adyen** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adyen](https://vinkius.com/mcp/adyen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
