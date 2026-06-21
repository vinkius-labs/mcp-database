# Teller MCP Server

Connect to your bank accounts, list transactions, check balances, and initiate payments via Teller API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/teller)

## Overview
**Category:** finance-accounting
**Tools Count:** 11

## Description
Connect your **Teller** enrollment to any AI agent and manage your financial data and payments through natural conversation.

### What you can do

- **Account Management** — List all financial accounts and fetch specific metadata for any connected bank account.
- **Identity Verification** — Retrieve owner information including names, addresses, phone numbers, and emails associated with the accounts.
- **Balances & Details** — Get real-time ledger and available balances, as well as sensitive account and routing numbers.
- **Transaction History** — Query historical ledger transactions with support for pagination and date filtering.
- **Payments** — Create payees and initiate payments (e.g., via Zelle) directly from your specified accounts.
- **Access Control** — Revoke authorization for specific accounts or the entire enrollment when needed.

### How it works

1. Subscribe to this server
2. Enter your Teller Access Token, Certificate, and Private Key
3. Start managing your banking data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate real-time banking data and payment flows into your AI-driven applications without building custom connectors.
- **Finance Teams** — automate transaction monitoring and balance checks across multiple institutions.
- **Personal Finance Users** — interact with your own bank data using natural language to track spending or verify account details.


## Available Tools
- **get_account_balances**: Get real-time ledger and available balances
- **get_account_details**: Get account and routing numbers
- **list_accounts**: List all accounts for the enrollment
- **create_payee**: Create a new payee for an account
- **delete_account**: Delete authorization for a specific account
- **delete_all_accounts**: Delete authorization for all accounts in the enrollment
- **get_account**: Get details for a specific account
- **get_identity**: Get identity information for accounts
- **initiate_payment**: g., via Zelle) from the specified account.

Initiate a payment from an account
- **list_institutions**: List supported financial institutions
- **list_transactions**: Supports pagination and date filtering.

List ledger transactions for an account


## Installation & Usage

To install and use the **Teller** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teller](https://vinkius.com/mcp/teller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
