# Highnote MCP Server

Automate card issuance and financial management via Highnote — manage account holders, cards, and transactions directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/highnote)

## Overview
**Category:** money-moves
**Tools Count:** 11

## Description
Connect your **Highnote** card platform to any AI agent and take full control of your card issuance, financial accounts, and ledger through natural conversation.

### What you can do

- **Account Holder Oversight** — List and retrieve details for individuals and businesses holding accounts in your program.
- **Card Management** — List virtual and physical cards, monitor their operational status, and freeze or close them directly from the chat.
- **Financial Account Monitoring** — Access real-time balances and metadata for all your financial ledger accounts.
- **Transaction Tracking** — List and inspect recent spending and processing transactions with detailed merchant metadata.
- **Ledger Insights** — Retrieve individual ledger entries for reconciliation and audit purposes.
- **Program Visibility** — List all available card products and programs configured in your Highnote account.

### How it works

1. Subscribe to this server
2. Enter your Highnote API Key and select your Environment (Test or Live)
3. Start managing your fintech program from Claude, Cursor, or any MCP-compatible client

No more manual querying of complex GraphQL schemas for simple account lookups. Your AI assistant acts as a dedicated Fintech Operations Lead or Card Program Manager.

### Who is this for?

- **Fintech Operations Managers** — instantly retrieve account balances and transaction details during reconciliation.
- **Customer Support for Neobanks** — check card statuses and freeze cards immediately upon customer request.
- **Product Managers** — monitor card issuance volume and program activity in real-time.


## Available Tools
- **get_financial_account**: Get detailed balance and metadata for a specific financial account
- **get_api_profile**: Retrieve information about the authenticated API user
- **get_payment_card_details**: Get detailed information for a specific card
- **get_transaction_details**: Get detailed metadata for a specific transaction
- **list_account_holders**: Use this to find the unique ID for a person or business.

List individuals and businesses who hold accounts in Highnote
- **list_card_products**: List the different card programs (e.g., Consumer, Fleet) available in your Highnote account
- **list_financial_accounts**: List all financial accounts and their current balances
- **list_ledger_entries**: Useful for reconciliation.

List individual ledger entries for a financial account
- **list_payment_cards**: Monitor card status and expiration details.

List virtual and physical cards issued in your program
- **list_financial_transactions**: List recent spending and processing transactions
- **update_card_status**: Valid statuses: ACTIVE, FROZEN, CLOSED.

Change the status of a card (e.g., ACTIVE, FROZEN, CLOSED)


## Installation & Usage

To install and use the **Highnote** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highnote](https://vinkius.com/mcp/highnote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
