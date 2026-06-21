# Brankas MCP Server

Manage open finance operations via Brankas API — process direct payments, send disbursements, and access bank statements from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/brankas)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect your **Brankas** Open Finance account to any AI agent and orchestrate your payments, payouts, and financial data workflows across Southeast Asia through natural conversation.

### What you can do

- **Direct Payments (Money-in)** — Initiate checkout sessions to accept instant account-to-account payments and track transaction statuses.
- **Disbursements (Money-out)** — Send payouts automatically through inter-bank or intra-bank transfers and monitor their progress.
- **Data Aggregation** — Retrieve real-time bank account balances, transaction history (statements), and identity data from consented users.

### How it works

1. Subscribe to this server
2. Enter your Brankas API Key and Environment (sandbox or production)
3. Start managing your open finance operations from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_checkout**: Create a new Direct payment checkout session
- **get_balance**: Retrieve linked bank account balances
- **get_identities**: Retrieve linked identity data
- **get_statement**: Retrieve linked bank statement data
- **get_transaction**: Get status of a Direct payment transaction
- **get_transfer_status**: Get status of a Disburse transfer
- **inter_bank_transfer**: Initiate an inter-bank disbursement (payout)
- **intra_bank_transfer**: Initiate an intra-bank disbursement (payout)


## Installation & Usage

To install and use the **Brankas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brankas](https://vinkius.com/mcp/brankas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
