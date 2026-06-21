# Alipay Open Platform MCP Server

Automate payment workflows via Alipay — create trades, process refunds, execute fund transfers, and reconcile billing ledgers natively from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/alipay-open-platform)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Bridge your intelligent agents directly into the sprawling financial infrastructure of **Alipay**, one of the world's largest payment ecosystems processing trillions annually across mobile commerce, lifestyle services, and B2C disbursements.

### What you can do

- **Payment Processing** — Create, query, close, and cancel trade orders dynamically handling full lifecycle management
- **Refund Management** — Execute full or partial refunds with reason tracking, automatically querying settlement status
- **Fund Transfers** — Dispatch B2C payouts to individual accounts verifying transfer completion and handling exceptions
- **Bill Reconciliation** — Download daily transaction summaries pulling structured accounting exports for automated book-keeping
- **User Identity** — Exchange OAuth authorization codes to access verified customer profiles securely

### How it works

1. Register as a developer on the [Alipay Open Platform](https://open.alipay.com/)
2. Create an Application to obtain your unique **App ID**
3. Generate an RSA2 key pair and upload the public key to the Alipay console
4. Paste the **App Private Key** below — the engine handles all RSA-SHA256 signature generation automatically per request

Eliminate manual API signature headaches entirely. Your AI agent now signs, dispatches, and parses every Alipay interaction with cryptographic precision leaving you free to focus on business logic.

### Who is this for?

- **E-commerce Operators** — automate order creation and refund processing across storefronts without switching dashboards constantly
- **Financial Controllers** — pull daily settlement bills reconciling ledgers automatically flagging discrepancies before human review
- **Growth Engineers** — integrate Alipay checkout flows into conversational commerce bots enabling frictionless mobile payments at scale


## Available Tools
- **cancel_trade**: Cancel a trade (rollback)
- **close_trade**: Close an unpaid Alipay trade
- **create_trade**: Create a new Alipay transaction/order
- **get_oauth_token**: Exchange authorization code for an OAuth Token
- **query_bill_download_url**: Query the download URL for accounting bills
- **query_trade**: Query the status of an Alipay trade
- **query_transfer**: Query the status of a fund transfer
- **query_user_info**: Query authorized Alipay user information
- **refund_trade**: Refund an Alipay transaction
- **transfer_fund**: Transfer funds to an Alipay user account


## Installation & Usage

To install and use the **Alipay Open Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alipay-open-platform](https://vinkius.com/mcp/alipay-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
