# Tatum (Blockchain Infra) MCP Server

Simplify blockchain development with Tatum — estimate fees, track portfolios, and manage real-time webhook subscriptions across multiple chains.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tatum-blockchain-infra)

## Overview
**Category:** developer-tools
**Tools Count:** 11

## Description
Connect your **Tatum** account to any AI agent to streamline blockchain infrastructure management. Access real-time data, gas estimates, and portfolio tracking across 40+ protocols through natural language.

### What you can do

- **Fee Estimation** — Get recommended fees or estimate gas for EVM transactions to optimize costs using `get_recommended_fee` and `estimate_evm_gas`.
- **Portfolio Tracking** — Retrieve balances for native assets, ERC-20 tokens, and NFTs across multiple addresses with `get_wallet_portfolio`.
- **Real-time Monitoring** — Create and manage webhook subscriptions for incoming/outgoing transactions using `create_subscription` and `list_subscriptions`.
- **Transaction History** — Query detailed historical data for specific blockchain addresses via `get_transaction_history`.
- **Exchange Rates** — Get live exchange rates between crypto and fiat currencies using `get_exchange_rate`.

### How it works

1. Subscribe to this server
2. Enter your Tatum API Key
3. Start querying blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Quickly estimate gas and debug transactions without leaving the IDE
- **DeFi Analysts** — Monitor portfolios and exchange rates in real-time through conversation
- **Ops Teams** — Automate webhook management for blockchain event monitoring


## Available Tools
- **cancel_subscription**: Cancel a webhook subscription
- **create_subscription**: ).

Create a webhook subscription
- **create_virtual_account**: Create a virtual account (off-chain ledger)
- **estimate_evm_gas**: Estimate EVM gas limit and price
- **estimate_transaction_fee**: ).

Estimate transaction fee
- **get_exchange_rate**: Get exchange rate for a crypto or fiat asset
- **get_recommended_fee**: Get recommended fee for a blockchain
- **get_transaction_history**: Get transaction history for an address
- **get_virtual_account_balance**: Get virtual account balance
- **get_wallet_portfolio**: Get wallet portfolio balances
- **list_subscriptions**: List active webhook subscriptions


## Installation & Usage

To install and use the **Tatum (Blockchain Infra)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tatum-blockchain-infra](https://vinkius.com/mcp/tatum-blockchain-infra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
