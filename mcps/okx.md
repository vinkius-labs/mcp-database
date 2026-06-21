# OKX MCP Server

Trade crypto and manage your OKX account via AI — check balances, track positions, and execute orders directly from your agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/okx)

## Overview
**Category:** data-analytics
**Tools Count:** 6

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


## Installation & Usage

To install and use the **OKX** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/okx](https://vinkius.com/mcp/okx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
