# ZeroHash MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zerohash)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zerohash-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zerohash-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Manage digital asset infrastructure via ZeroHash — list assets, manage accounts, create customers, and execute trades directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZeroHash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all supported stablecoins on ZeroHash."

**🤖 AI Agent:**
> I've retrieved the supported stablecoins. Currently, you can trade assets like USDC (on Ethereum and Solana), USDT, and PYUSD. Would you like to see the full details for any of these?

---

**👤 You:**
> "Check my current account balances for BTC and ETH."

**🤖 AI Agent:**
> Your current balances are: 1.25 BTC in your primary trading account and 15.0 ETH in your liquidity pool account. Do you need a breakdown of other assets?

---

**👤 You:**
> "Request a quote to buy 0.5 BTC using USD."

**🤖 AI Agent:**
> I've requested a quote for buying 0.5 BTC. The current rate is 65,000 USD per BTC, totaling 32,500 USD. This quote is valid for the next 30 seconds. Would you like to execute this trade?


## Installation & Usage

To install and use the **ZeroHash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zerohash](https://vinkius.com/mcp/zerohash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
