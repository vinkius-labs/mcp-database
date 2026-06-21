# Mono MCP Server

Automate financial data retrieval and payment orchestration via Mono — access account balances, transaction history, and initiate bank transfers directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mono)

## Overview
**Category:** finance-accounting
**Tools Count:** 5

## Description
Connect your **Mono** account to any AI agent to access real-time financial data and payment capabilities across African financial institutions through natural conversation.

### What you can do

- **Account Insights** — Fetch real-time balances, account numbers, and institution details for any linked account using `get_account`.
- **Transaction Analysis** — Query historical transaction data with filters for dates and types (credit/debit) via `get_transactions`.
- **Statement Retrieval** — Generate and download bank statements in JSON or PDF formats for auditing and reconciliation using `get_statement`.
- **Identity Verification** — Retrieve verified identity information including Full Name, BVN, and contact details with `get_identity`.
- **Payment Initiation** — Orchestrate direct bank transfers with custom references and descriptions using `initiate_payment`.

### How it works

1. Subscribe to this server
2. Enter your Mono Secret Key
3. Start managing financial data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate Mono features directly from your code editor to maintain development flow.
- **Financial Analysts** — Automate the collection of statements and transaction logs for faster reporting and auditing.
- **Operations Teams** — Verify user identities and initiate payouts through simple natural language commands.


## Available Tools
- **get_account**: Get Mono account details
- **get_identity**: Get identity information for a Mono account
- **initiate_payment**: Initiate a direct bank transfer
- **get_statement**: Get bank statement for a Mono account
- **get_transactions**: Get transactions for a Mono account


## Installation & Usage

To install and use the **Mono** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mono](https://vinkius.com/mcp/mono)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
