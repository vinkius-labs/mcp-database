# ZeroHash MCP Server

Manage digital asset infrastructure via ZeroHash — list assets, manage accounts, create customers, and execute trades directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zerohash)

## Overview
**Category:** finance-accounting
**Tools Count:** 12

## Description
Connect your **ZeroHash** API credentials to any AI agent to orchestrate digital asset workflows through natural language. ZeroHash provides the underlying infrastructure for crypto and stablecoin liquidity, custody, and settlement.

### What you can do

- **Asset & Account Discovery** — List supported assets and check real-time balances across account groups and types using `list_assets` and `list_accounts`.
- **Customer Onboarding** — Programmatically create new customer participants with full KYC data integration via `create_customer`.
- **Trading & Liquidity** — Request real-time quotes for asset pairs and execute trades instantly using `request_quote` and `execute_quote`.
- **Transfers & Deposits** — Manage crypto deposits, create transfers, and link external accounts for seamless movement of funds.
- **Transaction Auditing** — Query trade history and fetch specific trade metadata for reporting and compliance using `list_trades` and `get_trade`.

### How it works

1. Subscribe to this server
2. Enter your ZeroHash API Key, Private Key, and Passphrase
3. Start managing your digital asset operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Fintech Developers** — Test and integrate crypto workflows directly from your IDE without switching contexts.
- **Operations Managers** — Monitor account balances and trade history through simple conversational queries.
- **Compliance Officers** — Quickly retrieve participant data and trade records for auditing and reporting purposes.


## Available Tools
- **list_accounts**: List accounts and current balances
- **list_assets**: List supported assets on ZeroHash
- **create_customer**: Create a new customer participant
- **create_transfer**: Use a unique client_transfer_id for idempotency.

Create an internal transfer between participants/accounts
- **list_crypto_deposits**: List incoming crypto deposits
- **execute_quote**: Execute a previously requested quote
- **get_trade**: Retrieve detailed information for a specific trade
- **link_external_account**: Link a bank account or blockchain address
- **list_participants**: List participants
- **request_quote**: Request a quote for a trade
- **get_time**: Unauthenticated.

Get current ZeroHash server time
- **list_trades**: List trades


## Installation & Usage

To install and use the **ZeroHash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zerohash](https://vinkius.com/mcp/zerohash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
