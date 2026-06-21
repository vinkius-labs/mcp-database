# TrueLayer MCP Server

Manage open banking payments, payouts, and account data via TrueLayer — initiate transfers, check balances, and list transactions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/truelayer)

## Overview
**Category:** finance-accounting
**Tools Count:** 13

## Description
Connect your **TrueLayer** account to any AI agent to automate financial operations and open banking workflows through natural conversation.

### What you can do

- **Payments & Payouts** — Create instant bank transfers, process payouts, and handle refunds with full control over currency and beneficiaries.
- **Merchant Accounts** — List and inspect your TrueLayer-managed merchant accounts, check balances, and monitor transaction history.
- **Open Banking Data** — Retrieve real-time account balances, transaction lists, and verify account ownership from connected banks.
- **Recurring Payments** — Set up and manage Variable Recurring Payment (VRP) mandates for automated billing and subscriptions.
- **Provider Discovery** — List available banking providers and verify credentials across supported regions.

### How it works

1. Subscribe to this server
2. Enter your TrueLayer Access Token
3. Start managing your fintech operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate payment flows directly from your code editor without switching to a browser.
- **Finance Teams** — Monitor merchant account balances and reconcile transactions through simple conversational queries.
- **Operations Managers** — Automate payouts and refunds to customers using a dedicated AI financial assistant.


## Available Tools
- **create_mandate**: Create a Variable Recurring Payment (VRP) mandate
- **create_payment**: Requires amount, currency, payment method, beneficiary, and user details.

Create a new single payment
- **create_payout**: Can be closed-loop or open-loop.

Create a new payout
- **create_refund**: Cannot exceed the original payment amount.

Create a refund for a payment
- **get_data_account_balance**: Get balance for a data account
- **get_merchant_account**: Get details for a specific merchant account
- **list_data_account_transactions**: List transactions for a data account
- **list_data_accounts**: Requires user consent token.

List user bank accounts (Data API)
- **list_merchant_account_transactions**: List transactions for a merchant account
- **list_merchant_accounts**: List TrueLayer merchant accounts
- **list_payment_sources**: List payment sources for a merchant account
- **list_providers**: List supported bank providers
- **verify_account**: Verify account ownership


## Installation & Usage

To install and use the **TrueLayer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truelayer](https://vinkius.com/mcp/truelayer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
