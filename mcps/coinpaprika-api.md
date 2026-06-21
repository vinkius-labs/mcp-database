# CoinPaprika API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coinpaprika-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coinpaprika-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coinpaprika-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access cryptocurrency data — audit coins, markets, and exchanges via AI.

## Description
Empower your AI agent to orchestrate your entire digital asset research and market auditing workflow with the **CoinPaprika API**, the comprehensive source for global cryptocurrency data. By connecting CoinPaprika to your agent, you transform complex market searches into a natural conversation. Your agent can instantly retrieve coin metadata, audit OHLCV price data, and query exchange lists without you ever touching a financial terminal. Whether you are conducting investment research or monitoring global market caps, your agent acts as a real-time crypto analyst, ensuring your data is always verified and precise.

### What you can do

- **Coin Auditing** — Retrieve high-resolution metadata for thousands of cryptocurrencies and maintain a clear view of coin rank, type, and status.
- **Market Oversight** — Audit the latest OHLCV (Open, High, Low, Close, Volume) data for specific coins to understand price intensity instantly.
- **Exchange Discovery** — Browse supported cryptocurrency exchanges to understand the distribution of liquidity across the global industry.
- **Global Intelligence** — Retrieve market-wide overview metadata to assist in deep-dive macroeconomic classification.
- **Live Tickers & Events** — Access real-time price tickers, upcoming project events, and mapped trading markets to build a comprehensive view of asset liquidity.

### How it works

1. Subscribe to this server
2. No API Key required (CoinPaprika is a free and open service)
3. Start managing your digital asset intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Analysts & Traders** — monitor coin performance and retrieve official market metadata straight from your workflow.
- **Web3 Developers** — verify asset availability and audit exchange patterns without manual searching.
- **Investors** — perform rapid audits of global market caps and identify relevant asset markers through natural language.
- **Operations Leads** — automate financial data querying to orchestrate cross-functional investment teams smoothly.


## Available Tools
- **get_coin_details**: Get full metadata and project details for a specific coin by ID
- **get_coin_events**: Get recent and upcoming events for a specific cryptocurrency
- **get_coin_exchanges**: Get all exchanges where a specific coin is traded
- **get_coin_markets**: Get all active trading markets and pairs for a specific coin
- **get_coin_ohlcv_latest**: Get the latest OHLCV (Open, High, Low, Close, Volume) data for a coin
- **get_global_market_overview**: Get an overview of the entire cryptocurrency market performance
- **get_coin_ticker**: Get real-time price and ticker data for a specific coin
- **list_all_coins**: Useful for mapping coin IDs.

List all available cryptocurrencies in the CoinPaprika database
- **list_crypto_exchanges**: List all cryptocurrency exchanges supported by CoinPaprika
- **list_all_tickers**: List current prices and ticker data for all active coins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinPaprika API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for 'Bitcoin' using CoinPaprika."

**🤖 AI Agent:**
> I've retrieved the details for Bitcoin (ID: btc-bitcoin)! It is currently ranked #1 with a 'coin' type status. It is identified as an active asset. Would you like the latest OHLCV price data or the global market overview?

---

**👤 You:**
> "What is the latest price for 'Ethereum'?"

**🤖 AI Agent:**
> I've checked the latest OHLCV data for Ethereum. The closing price is identified as 2,500 USD with a 24-hour volume of [Volume]. I can assist you with more asset metadata if you'd like.

---

**👤 You:**
> "List top cryptocurrency exchanges."

**🤖 AI Agent:**
> I've retrieved the exchange catalog from CoinPaprika! There are hundreds of exchanges listed, including Binance, Coinbase, and Kraken. I can provide the unique ID and status for each of these platforms to assist in your liquidity audit.


## Installation & Usage

To install and use the **CoinPaprika API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinpaprika-api](https://vinkius.com/mcp/coinpaprika-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
