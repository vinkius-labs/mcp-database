# Authorize.net MCP Server

Manage payments, transactions, and customer profiles via Authorize.net — the trusted payment gateway directly via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/authorizenet-1)

## Overview
**Category:** money-moves
**Tools Count:** 10

## Description
Connect your **Authorize.net** merchant account to any AI agent and manage your entire payment lifecycle through natural conversation.

### What you can do

- **Transaction Management** — Authorize, capture, refund, and void transactions with full audit trails and security
- **Financial Reporting** — List transactions from settled batches, unsettled queues, and analyze processing performance
- **Customer Profiles** — Retrieve and manage secure customer payment information and subscription profiles
- **Batch Insights** — Monitor daily settlement statistics and high-level performance metrics for your merchant account

### How it works

1. Subscribe to this server
2. Enter your Authorize.net API Login ID and Transaction Key
3. Start managing your payments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — audit recent transactions, check settlement statuses, and process refunds without manual dashboard navigation
- **E-commerce Managers** — monitor payment health and manage customer billing profiles directly from their workspace
- **Developers** — test payment flows in sandbox and audit transaction metadata through natural language commands


## Available Tools
- **create_transaction**: You must provide the transaction type (e.g., authCaptureTransaction) and the request body.

Create a new payment transaction
- **get_batch_statistics**: Get statistics for a specific batch
- **get_customer_profile**: Retrieve a customer profile by ID
- **get_settled_batch_list**: Retrieve a list of settled batches for a date range
- **get_transaction_details**: Get complete information for a specific transaction
- **get_transaction_list**: List transactions for a specific settled batch
- **get_unsettled_transaction_list**: List the most recent unsettled transactions
- **list_customer_profiles**: Retrieve a list of all customer profile IDs
- **refund_transaction**: Refund a settled transaction
- **void_transaction**: Void an unsettled transaction


## Installation & Usage

To install and use the **Authorize.net** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/authorizenet-1](https://vinkius.com/mcp/authorizenet-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
