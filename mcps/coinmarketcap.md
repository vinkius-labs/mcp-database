# CoinMarketCap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coinmarketcap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coinmarketcap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coinmarketcap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Enable your AI agent to query crypto prices, market rankings, and currency conversions via the CoinMarketCap API.

## Description
Connect your AI to **CoinMarketCap**, the world's most-referenced crypto price-tracking platform.

### What you can do

- **Market Rankings** — List the top cryptocurrencies by market cap, volume, or price change.
- **Price Conversion** — Convert between hundreds of cryptocurrencies and dozens of fiat currencies.
- **API Usage** — Check your API key's remaining credits and usage stats.

### How it works

1. Add the CoinMarketCap integration to your AI toolset.
2. Provide your API Key (from pro.coinmarketcap.com).
3. Query crypto market data via natural language.

### Who is this for?

- **Traders** — Get real-time prices and rankings without leaving the chat.
- **Developers** — Integrate crypto pricing into workflows and monitor API usage.
- **Analysts** — Pull market data for research and portfolio tracking.


## Available Tools
- **get_global_metrics**: Retrieve aggregate market data for the entire cryptocurrency market
- **get_id_map**: Retrieve a mapping of symbols/names to unique CMC IDs
- **get_key_info**: Check your API keys usage, remaining credits, and rate limits
- **get_metadata**: Retrieve static metadata for one or more cryptocurrencies (logo, description, etc.)
- **get_quotes**: Retrieve the latest market quotes for one or more cryptocurrencies
- **list_exchanges**: Retrieve a ranked list of all cryptocurrency exchanges
- **list_listings**: Retrieve a paginated list of all active cryptocurrencies with latest market data
- **price_conversion**: Convert an amount of one currency to another using latest market prices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinMarketCap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 10 cryptocurrencies by market cap."

**🤖 AI Agent:**
> Top 10 by market cap:
1. Bitcoin (BTC) — $1.2T, $67,420
2. Ethereum (ETH) — $410B, $3,415
3. Tether (USDT) — $110B, $1.00
...
Would you like price details or 24h change for any?

---

**👤 You:**
> "Convert 1.5 BTC to EUR."

**🤖 AI Agent:**
> 1.5 BTC = €94,230.45 EUR (rate: €62,820.30/BTC). Last updated: 2 minutes ago.

---

**👤 You:**
> "Get the historical listing data for Dogecoin launched on CoinMarketCap."

**🤖 AI Agent:**
> Dogecoin (DOGE) was listed on CoinMarketCap on Dec 15, 2013, with an initial tracked market cap around $3.5M. Present market cap is $16.9B.


## Installation & Usage

To install and use the **CoinMarketCap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinmarketcap](https://vinkius.com/mcp/coinmarketcap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
