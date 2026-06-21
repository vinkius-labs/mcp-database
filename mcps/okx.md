# OKX MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/okx)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/okx-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/okx-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Trade crypto and manage your OKX account via AI — check balances, track positions, and execute orders directly from your agent.

## Description
Connect your **OKX** trading account to any AI agent to monitor markets and manage your portfolio through natural language.

### What you can do

- **Market Data** — Retrieve available instruments for spot, margin, futures, and options trading using `get_instruments`.
- **Account Monitoring** — Fetch real-time asset balances with `get_balance` and track active positions across different instrument types with `get_positions`.
- **Order Management** — Place new trade orders (limit, market, etc.) via `place_order`, amend existing ones with `amend_order`, or cancel pending orders instantly using `cancel_order`.
- **Flexible Trading** — Support for various trade modes including cash, cross, and isolated margin directly from your conversation.

### How it works

1. Subscribe to this server
2. Enter your OKX API Key, Secret Key, and Passphrase
3. Start trading and monitoring your portfolio from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders** — execute orders and check positions without switching between multiple exchange tabs or mobile apps.
- **Developers** — integrate trading capabilities into automated workflows or code editors to monitor exposure while working.
- **Portfolio Managers** — get quick summaries of balances and risk exposure across different asset classes using natural language queries.


## Available Tools
- **amend_order**: Requires instrument ID and either order ID or client order ID.

Amend an existing incomplete order
- **get_balance**: Can be filtered by specific currencies.

Retrieve asset balances in the trading account
- **cancel_order**: Requires instrument ID and either order ID or client order ID.

Cancel an incomplete order
- **get_instruments**: Can be filtered by instrument type.

Retrieve available instruments for the account
- **place_order**: Requires instrument ID, trade mode, side, order type, and size.

Place a new trade order
- **get_positions**: Can be filtered by instrument type, instrument ID, or position ID.

Retrieve active positions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OKX** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my current USDT and BTC balance on OKX."

**🤖 AI Agent:**
> I've retrieved your balances. You currently have 1,250.50 USDT available and 0.045 BTC. Would you like to see balances for any other assets?

---

**👤 You:**
> "List all my active futures positions."

**🤖 AI Agent:**
> You have one active position: BTC-USDT-SWAP (Long) with a size of 0.1 BTC at an entry price of 65,000. Your current unrealized PnL is +$120.00.

---

**👤 You:**
> "Place a market buy order for 0.01 BTC on the BTC-USDT spot market."

**🤖 AI Agent:**
> Market buy order for 0.01 BTC on BTC-USDT has been placed successfully. Order ID: 192837465. Trade mode: cash.


## Installation & Usage

To install and use the **OKX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/okx](https://vinkius.com/mcp/okx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
