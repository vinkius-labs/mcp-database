# Highnote MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/highnote)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/highnote-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/highnote-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate card issuance and financial management via Highnote — manage account holders, cards, and transactions directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Highnote** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all financial accounts and show their current balances."

**🤖 AI Agent:**
> I've retrieved your financial accounts. You have 3 active ledgers: 'Main Operations' ($145,000.00), 'Fleet Fuel Card Fund' ($12,500.00), and 'Marketing Expenses' ($5,000.00). Would you like to see the recent ledger entries for any of these?

---

**👤 You:**
> "Show the last 5 transactions for card ending in 4492."

**🤖 AI Agent:**
> Accessing transaction history... For card **** 4492, the 5 most recent transactions include: $42.50 at 'Shell Station', $12.99 at 'Starbucks', and $150.00 at 'Amazon'. All transactions are currently in 'CLEARED' status. Should I retrieve the full details for the Amazon purchase?

---

**👤 You:**
> "Freeze card ID 'card_992' immediately."

**🤖 AI Agent:**
> Card frozen! I've successfully updated the status of card card_992 to 'FROZEN'. This card will no longer accept new transactions until it is unfrozen. Would you like me to notify the account holder via email?


## Installation & Usage

To install and use the **Highnote** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highnote](https://vinkius.com/mcp/highnote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
