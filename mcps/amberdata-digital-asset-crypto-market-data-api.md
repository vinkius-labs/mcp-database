# Amberdata (Digital Asset & Crypto Market Data API) MCP Server

Access institutional-grade crypto market data, on-chain metrics, and DeFi insights directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amberdata-digital-asset-crypto-market-data-api)

## Overview
**Category:** data-analytics
**Tools Count:** 28

## Description
Connect your **Amberdata** account to any AI agent to access comprehensive digital asset data through natural conversation. This server provides a unified interface for market data, blockchain analytics, and DeFi protocols.

### What you can do

- **Market Data** — Fetch real-time and historical Spot, Futures, and Options tickers, trades, and OHLCV data across major exchanges.
- **Order Book Analysis** — Access full L2 order book snapshots and incremental event deltas to analyze market depth and liquidity.
- **On-chain Metrics** — Query blockchain-level data including address balances, token transfers, and transaction metrics for major networks.
- **DeFi Insights** — Inspect DEX information, lending protocol metrics, and liquidity pool data directly.
- **Reference Rates** — Retrieve SOC I/II compliant benchmark prices for major assets like BTC and ETH.

### How it works

1. Subscribe to this server
2. Enter your Amberdata API Key
3. Start querying crypto markets and blockchain data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders & Analysts** — Instantly retrieve market prices, spreads, and volume metrics without switching between exchange tabs.
- **Blockchain Developers** — Check address balances and transaction history directly from your coding environment.
- **DeFi Researchers** — Monitor lending protocols and DEX activity using natural language queries.


## Available Tools
- **get_address_balances_latest**: Get current native account balance
- **get_address_token_balances_latest**: Get current ERC-20 token holdings
- **get_address_token_transfers**: Get historical token transfer events for an address
- **get_blockchain_metrics_latest**: Get latest block and transaction metrics
- **get_blocks_metrics_historical**: Get historical block-level metrics
- **get_defi_dex_information**: Get list of supported liquidity pools and protocols
- **get_defi_lending_assets_metrics_summary**: Get aggregated insights into lending asset markets
- **get_defi_lending_protocols_information**: Get supported lending protocols (Aave, Compound, MakerDAO, etc.)
- **get_defi_market_ohlcv_latest**: Get latest OHLCV for a DEX pair
- **get_defi_market_trades_historical**: Get historical tick-by-tick DEX trades
- **get_futures_ohlcv**: Get aggregated OHLCV for futures
- **get_futures_order_book_snapshots**: Get order book snapshots for futures
- **get_futures_tickers**: Get historical/latest tickers for futures/perpetuals
- **get_futures_trades**: Get tick-by-tick trades for futures
- **get_options_ohlcv**: Get aggregated OHLCV for options
- **get_options_tickers**: Get tickers including Greeks and Implied Volatility for options
- **get_options_trades**: Get tick-by-tick trades for options
- **get_spot_bid_ask_spread**: Get absolute and percentage spread analytics
- **get_spot_ohlcv**: Get aggregated Open, High, Low, Close, Volume for a spot instrument
- **get_spot_order_book_events**: Get incremental L2 order book updates (deltas) for a spot instrument
- **get_spot_order_book_snapshots**: Get 1-minute snapshots of the full order book for a spot instrument
- **get_spot_reference_rates**: Get benchmark prices for BTC/ETH (SOC I/II compliant)
- **get_spot_tickers**: Get historical/latest best bid/ask (BBO) for a spot instrument
- **get_spot_trade_frequency**: Get aggregated trade counts by size category
- **get_spot_trade_pressure**: Get net trade data (buy vs sell aggressors)
- **get_spot_trades**: Get tick-by-tick executed transactions for a spot instrument
- **get_spot_vwap_twap**: Get Volume/Time Weighted Average Price
- **get_transactions_metrics_historical**: Get historical transaction-level metrics


## Installation & Usage

To install and use the **Amberdata (Digital Asset & Crypto Market Data API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amberdata-digital-asset-crypto-market-data-api](https://vinkius.com/mcp/amberdata-digital-asset-crypto-market-data-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
