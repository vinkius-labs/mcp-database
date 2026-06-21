# Brave New Coin MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brave-new-coin)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brave-new-coin-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brave-new-coin-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access institutional-grade cryptocurrency data via Brave New Coin — track prices, markets, and historical data directly from any AI agent.

## Description
Connect your AI agent to the **Brave New Coin (BNC)** API and orchestrate your cryptocurrency research and trading workflows through natural conversation.

### What you can do

- **Real-time Pricing** — Retrieve the latest Global Weighted Average (GWA) prices and 24h volumes for major cryptocurrencies.
- **Asset Discovery** — List all supported digital assets and retrieve their unique identifiers.
- **Market Analysis** — List exchanges and trading pairs where specific assets are actively traded.
- **Historical Data** — Fetch OHLCV (Open, High, Low, Close, Volume) data for backtesting and technical analysis.
- **Advanced Metrics** — Access Volume Weighted Average Price (VWAP) and detailed GWA components.

### How it works

1. Subscribe to this server
2. Enter your Brave New Coin RapidAPI Key
3. Start analyzing the crypto market from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_asset**: Get details of a specific asset
- **get_gwa**: Get Global Weighted Average details
- **get_market**: Get details of a specific market
- **get_ohlcv**: Get historical Open High Low Close Volume data
- **get_ticker**: Get the latest Global Weighted Average price/ticker
- **get_vwap**: Get Volume Weighted Average Price
- **list_assets**: List all supported crypto assets
- **list_markets**: List exchanges/markets where an asset is traded


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brave New Coin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest ticker price for BTC."

**🤖 AI Agent:**
> The latest Global Weighted Average price for Bitcoin (BTC) is $64,230.15 USD.

---

**👤 You:**
> "List the markets where Ethereum (ETH) is traded."

**🤖 AI Agent:**
> I've retrieved the markets for ETH. Top exchanges include Binance (ETH/USDT), Coinbase (ETH/USD), and Kraken (ETH/USD).

---

**👤 You:**
> "Get historical OHLCV data for the Binance BTC/USDT market."

**🤖 AI Agent:**
> Retrieving data... The last closed candle shows Open: $64,000, High: $64,500, Low: $63,800, Close: $64,200, Volume: 1500 BTC.


## Installation & Usage

To install and use the **Brave New Coin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brave-new-coin](https://vinkius.com/mcp/brave-new-coin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
