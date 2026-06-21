# Alpaca Trading MCP Server

Trade stocks and crypto, access real-time market data, and manage your Alpaca brokerage account directly through any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/alpaca-trading)

## Overview
**Category:** money-moves
**Tools Count:** 14

## Description
Connect your **Alpaca Markets** account to your AI agent to automate trading strategies and monitor market movements through natural language.

### What you can do

- **Order Execution** — Place market, limit, or stop orders for stocks and crypto assets using `create_order` and manage them with `delete_all_orders`.
- **Market Intelligence** — Retrieve historical bars, latest quotes, and trade data for stocks and crypto using tools like `get_stocks_bars` and `get_latest_stocks_quotes`.
- **Order Tracking** — Query your order history with advanced filters like status, symbols, and timeframes via `get_orders`.
- **Account Management** — Check your broker account details and update configurations such as fractional trading or shorting permissions with `update_account_configs`.
- **Asset Discovery** — List available assets and their trading status directly from the Alpaca exchange.

### How it works

1. Subscribe to this server
2. Enter your Alpaca API Key ID and Secret Key
3. Start trading and analyzing markets from Claude, Cursor, or any MCP-compatible client

Your AI acts as a sophisticated trading terminal, capable of executing complex orders and fetching deep market analytics without you ever leaving your workflow.

### Who is this for?

- **Quant Traders** — automate the execution of strategies and fetch historical data for backtesting analysis.
- **Retail Investors** — check portfolio status and place quick trades using simple conversational commands.
- **Developers** — integrate financial market data and trading capabilities directly into coding environments.


## Available Tools
- **create_broker_account**: Requires contact, identity, disclosures, and agreements objects.

Create a new broker account
- **create_order**: Create a new trading order
- **delete_all_orders**: Returns a 207 Multi-Status.

Delete all open orders
- **get_assets**: List all tradable assets
- **get_broker_account**: Get broker account by ID
- **get_crypto_bars**: Get historical bars for crypto
- **get_latest_stocks_quotes**: Get latest quotes for stocks
- **get_latest_stocks_trades**: Get latest trades for stocks
- **get_orders**: Get all orders
- **get_stocks_bars**: Get historical bars for stocks
- **get_stocks_quotes**: Get historical quotes for stocks
- **get_stocks_trades**: Get historical trades for stocks
- **issue_token**: Issue OAuth2 tokens for machine-to-machine authentication
- **update_account_configs**: Update account configurations


## Installation & Usage

To install and use the **Alpaca Trading** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alpaca-trading](https://vinkius.com/mcp/alpaca-trading)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
