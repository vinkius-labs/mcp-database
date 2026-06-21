# Braintree MCP Server

Process and manage payments via Braintree GraphQL API — search transactions, manage customers, and issue refunds directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/braintree)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect your **Braintree** gateway account to any AI agent and orchestrate your global payment and checkout workflows through natural conversation.

### What you can do

- **Transaction Oversight** — Search and list recent transactions or retrieve detailed metadata for specific payments.
- **Payment Lifecycle Management** — Charge payment methods, capture authorized funds, void pending transactions, and issue full or partial refunds.
- **Customer Data Orchestration** — Search your customer vault by email and retrieve detailed billing profiles and saved payment methods.
- **GraphQL Power** — Leverage the flexibility of Braintree's modern GraphQL API for precise data retrieval.

### How it works

1. Subscribe to this server
2. Enter your Braintree Public Key, Private Key, and Environment (sandbox or production)
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **capture_transaction**: Capture an authorized transaction
- **charge_payment_method**: Charge a payment method
- **get_customer**: Get details of a specific customer
- **get_transaction**: Get details of a specific transaction
- **refund_transaction**: Optionally provide a partial amount.

Refund a settled transaction
- **search_customers**: Search for customers
- **search_transactions**: Search for recent transactions
- **void_transaction**: Void an authorized transaction


## Installation & Usage

To install and use the **Braintree** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/braintree](https://vinkius.com/mcp/braintree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
