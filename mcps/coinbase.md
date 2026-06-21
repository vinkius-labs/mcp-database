# Coinbase MCP Server

Get real-time cryptocurrency prices, exchange rates and currency info — BTC, ETH, SOL and more.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coinbase)

## Overview
**Category:** money-moves
**Tools Count:** 8

## Description
Connect to **Coinbase** and access real-time cryptocurrency market data through natural conversation — no API key needed for public price data.

### What you can do

- **Buy/Sell Prices** — Get current buy and sell prices for any trading pair
- **Spot Prices** — Get mid-market spot prices (historical prices supported)
- **Multi-Asset Prices** — Get prices for multiple pairs in one call
- **Currencies** — Browse all supported cryptocurrencies and fiat currencies
- **Exchange Rates** — Get exchange rates from any base currency
- **Payment Methods** — View available payment methods on your account

### How it works

1. Subscribe to this server
2. No API key needed for public price data
3. Start exploring crypto prices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders** — check real-time buy/sell prices and spreads before trading
- **Investors** — track crypto prices, compare exchange rates and monitor market data
- **Developers** — integrate crypto price data into apps and dashboards


## Available Tools
- **get_buy_price**: Returns the total price including Coinbase fees. Common pairs: BTC-USD, ETH-USD, SOL-USD, USDC-USD. Prices update in real-time and are only valid for seconds.

Get the current buy price for a cryptocurrency pair
- **get_currencies**: Returns currency codes, names, min/max precision, sort order and whether the currency is a cryptocurrency or fiat.

Get all supported cryptocurrencies and fiat currencies
- **get_exchange_rates**: Returns rates for crypto and fiat currencies. Useful for currency conversion.

Get current exchange rates for a currency
- **get_payment_methods**: Returns bank accounts, debit cards and other payment options with their IDs, types, limits and verification status.

Get available payment methods
- **get_public_prices**: Provide comma-separated pairs (e.g. "BTC-USD,ETH-USD,SOL-USD"). Useful for comparing prices across multiple assets quickly.

Get buy, sell and spot prices for multiple cryptocurrency pairs at once
- **get_sell_price**: Returns the total price you would receive including Coinbase fees. Common pairs: BTC-USD, ETH-USD, SOL-USD.

Get the current sell price for a cryptocurrency pair
- **get_spot_price**: This is the mid-market price without buy/sell spread. Optional date parameter for historical prices (YYYY-MM-DD UTC).

Get the current spot (market) price for a cryptocurrency pair
- **get_time**: Useful for synchronizing requests and verifying API connectivity.

Get the current Coinbase API server time


## Installation & Usage

To install and use the **Coinbase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinbase](https://vinkius.com/mcp/coinbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
