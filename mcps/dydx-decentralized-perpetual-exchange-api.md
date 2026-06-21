# dYdX (Decentralized Perpetual Exchange API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dydx-decentralized-perpetual-exchange-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dydx-decentralized-perpetual-exchange-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dydx-decentralized-perpetual-exchange-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Trade perpetuals on dYdX v4 — access markets, orderbooks, and manage your decentralized trading account directly from any AI agent.

## Description
Connect your **dYdX** account to any AI agent to monitor markets and execute trades on the leading decentralized perpetual exchange. This server provides full access to the dYdX v4 (dYdX Chain) infrastructure.

### What you can do

- **Market Analysis** — List all available markets, fetch detailed market info, and analyze 24h rolling statistics.
- **Real-time Data** — Access L2 orderbooks, recent public trades, and historical OHLCV candlestick data for technical analysis.
- **Account Management** — Check balances, equity, and open positions for any dYdX Chain address.
- **Trading Operations** — Place limit or market orders, cancel existing orders, and track your order history or fills through natural language.

### How it works

1. Subscribe to this server
2. Enter your dYdX API Key, Secret, and Passphrase
3. Start trading and analyzing crypto markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders** — execute trades and monitor positions without leaving your research environment or terminal.
- **DeFi Analysts** — pull real-time market data and orderbook depth directly into your analysis tools.
- **Developers** — test trading strategies and inspect account states using natural language commands.


## Available Tools
- **v3_create_order**: Requires authentication.

Place a new order on dYdX v3
- **v3_get_accounts**: Requires authentication.

Get account information on dYdX v3
- **v3_get_orderbook**: Get the current L2 orderbook for a dYdX v3 market
- **v3_list_markets**: List all available markets on dYdX v3
- **v4_cancel_order**: Requires authentication.

Cancel an open order by ID on dYdX v4
- **v4_create_order**: Requires authentication.

Place a new limit or market order on dYdX v4
- **v4_get_account**: Requires authentication.

Get account balances, positions, and equity on dYdX v4
- **v4_get_candles**: Get historical OHLCV data for a dYdX v4 market
- **v4_get_market**: g., BTC-USD).

Get details for a specific dYdX v4 market
- **v4_get_orderbook**: Get the current L2 orderbook for a dYdX v4 market
- **v4_get_stats**: Get 24h statistics for a dYdX v4 market
- **v4_get_trades**: Get recent public trades for a dYdX v4 market
- **v4_list_fills**: List recent trade fills for the account on dYdX v4
- **v4_list_markets**: List all available perpetual markets on dYdX v4
- **v4_list_orders**: List active and historical orders for the account on dYdX v4
- **v4_list_positions**: List all open positions on dYdX v4


## 💬 Prompt Examples

Here are some examples of how you can interact with the **dYdX (Decentralized Perpetual Exchange API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active markets on dYdX v4."

**🤖 AI Agent:**
> I've retrieved the active markets. Currently, there are several pairs available including BTC-USD, ETH-USD, and SOL-USD. Would you like details on a specific one?

---

**👤 You:**
> "What is the current orderbook for ETH-USD?"

**🤖 AI Agent:**
> Fetching the L2 orderbook for ETH-USD... The best bid is at $2,450.50 and the best ask is at $2,450.60. There is significant liquidity within the 1% range.

---

**👤 You:**
> "Show my open positions and account balance for address dydx1..."

**🤖 AI Agent:**
> Checking account state... You have one open long position in BTC-USD (size: 0.1 BTC). Your total equity is $5,200.40 with a buying power of $15,000.


## Installation & Usage

To install and use the **dYdX (Decentralized Perpetual Exchange API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dydx-decentralized-perpetual-exchange-api](https://vinkius.com/mcp/dydx-decentralized-perpetual-exchange-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
