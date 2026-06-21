# Kraken MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kraken-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kraken-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kraken-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Access real-time crypto market data, account balances, and trade history from Kraken directly within your AI agent.

## Description
Connect your **Kraken** account to any AI agent to monitor the cryptocurrency markets and manage your portfolio through natural language.

### What you can do

- **Market Data** — Fetch real-time ticker information, OHLC charts, and order book depth for any supported asset pair.
- **Account Overview** — Check your spot and trade balances across all held assets instantly.
- **Order Tracking** — List and inspect your open and closed orders to stay on top of your trading activity.
- **System Monitoring** — Verify Kraken's system status and server time to ensure optimal trading conditions.
- **Asset Discovery** — Query available assets and tradable pairs to identify new market opportunities.

### How it works

1. Subscribe to this server
2. Enter your Kraken API Key and API Secret
3. Start analyzing crypto markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders** — Get instant price updates and check balances without switching to a browser or mobile app.
- **Financial Analysts** — Pull historical OHLC data and market spreads directly into your analysis workflow.
- **Developers** — Test market data queries and monitor account status straight from your coding environment.


## Available Tools
- **futures_get_history**: Get Trade History (Futures)
- **futures_get_orderbook**: Get Orderbook (Futures)
- **futures_get_tickers**: Get Tickers (Futures)
- **futures_send_order**: Send Order (Futures)
- **spot_add_order**: Add Order
- **spot_cancel_all_orders_after**: Cancel All Orders After X
- **spot_cancel_all**: Cancel All Orders
- **spot_cancel_order**: Cancel Order
- **spot_get_asset_pairs**: Get Tradable Asset Pairs
- **spot_get_assets**: Get Asset Info
- **spot_get_balance**: Get Account Balance
- **spot_get_closed_orders**: Get Closed Orders
- **spot_get_depth**: Get Order Book
- **spot_get_ledgers**: Get Ledgers Info
- **spot_get_ohlc**: Get OHLC Data
- **spot_get_open_orders**: Get Open Orders
- **spot_get_open_positions**: Get Open Positions
- **spot_get_spread**: Get Recent Spreads
- **spot_get_system_status**: Get System Status
- **spot_get_ticker**: Get Ticker Information
- **spot_get_time**: Get Server Time
- **spot_get_trade_balance**: Get Trade Balance
- **spot_get_trade_volume**: Get Trade Volume
- **spot_get_trades_history**: Get Trades History
- **spot_get_trades**: Get Recent Trades
- **spot_get_websockets_token**: Get WebSockets Token
- **spot_query_orders**: Query Orders Info
- **spot_query_trades**: Query Trades Info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kraken** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current market price and 24h volume for Ethereum (ETH/USD)?"

**🤖 AI Agent:**
> I've checked the Kraken ticker for XETHZUSD. The last trade was at $2,450.20 with a 24-hour volume of 15,420 ETH. The current spread is $0.10.

---

**👤 You:**
> "Show me my current Kraken account balances."

**🤖 AI Agent:**
> Fetching your balances... You currently hold 0.5 BTC, 10 ETH, and 5,000 USD in your spot account.

---

**👤 You:**
> "Check if there are any open orders on my account."

**🤖 AI Agent:**
> I found one open limit order to sell 0.1 BTC at $70,000. It is currently 'open' and has not been partially filled yet.


## Installation & Usage

To install and use the **Kraken** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kraken-alternative](https://vinkius.com/mcp/kraken-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
