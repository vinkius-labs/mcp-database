# CoinGecko MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coingecko-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time cryptocurrency prices, market data, and on-chain analytics from the world's leading crypto data aggregator.

## Description
Connect your **CoinGecko** API to any AI agent to transform it into a powerful financial analyst. Get instant access to thousands of tokens, global market statistics, and deep exchange data through natural conversation.

### What you can do

- **Real-time Pricing** — Fetch current prices for thousands of coins across multiple fiat and crypto currencies using `get_simple_price`.
- **Market Insights** — Analyze market caps, 24h volumes, and price changes with `list_coins_markets` to identify market trends.
- **On-chain Intelligence** — Inspect specific tokens and networks directly from the blockchain using `get_onchain_token` and `list_onchain_networks`.
- **Trending & Global Data** — Stay ahead of the curve by querying `get_trending` coins or checking the `get_global` market overview.
- **Exchange & NFT Data** — List active exchanges, check trading pairs with `get_coin_tickers`, or explore NFT floor prices and contract data.

### How it works

1. Subscribe to this server
2. Enter your CoinGecko API Key (Demo or Pro)
3. Start querying crypto data from Claude, Cursor, or any MCP-compatible client

No more manual searching through charts. Your AI can now calculate portfolio values, find trending assets, and monitor market volatility in real-time.

### Who is this for?

- **Crypto Traders** — instantly get price updates and market sentiment without leaving your terminal or chat.
- **Web3 Developers** — fetch contract addresses, platform IDs, and on-chain data directly into your coding environment.
- **Financial Analysts** — automate the collection of historical data and global market metrics for reporting.


## Available Tools (29)
- **get_coin_market_chart_range**: Get historical market data within a range of timestamp
- **get_coin_market_chart**: Get historical market data
- **get_coin_ohlc**: Get coin OHLC data
- **get_coin_tickers**: Get coin tickers
- **get_coin**: including exchange tickers) for a coin.

Get current data for a coin
- **list_coins**: List all supported coins id, name and symbol
- **list_coins_markets**: List all supported coins price, market cap, volume, and market related data
- **get_exchange_tickers**: Get exchange tickers
- **get_exchange**: Get exchange volume in BTC and tickers
- **get_exchange_volume_chart**: Get volume chart data for an exchange
- **list_exchanges_markets**: List all supported markets id and name
- **list_exchanges**: List all exchanges
- **get_global_defi**: Get top 100 cryptocurrencies global DeFi data
- **get_global**: Get cryptocurrency global data
- **get_nft_by_contract**: Get NFT data by contract address
- **get_nft**: ) for an NFT collection.

Get current data for an NFT collection
- **list_nfts**: List all supported NFT collections
- **list_onchain_dexes**: List supported DEXes on a network
- **list_onchain_networks**: List all supported networks on GeckoTerminal
- **get_onchain_pool**: Get liquidity pool data by address
- **get_onchain_pool_trades**: Get latest trades from a pool
- **get_onchain_token**: Get token data by contract address
- **get_public_treasury**: g., bitcoin, ethereum).

Get public companies holdings for a specific coin
- **get_simple_price**: Get current price of cryptocurrencies
- **get_simple_token_price**: Get current price of tokens for a given platform
- **get_supported_vs_currencies**: Get list of supported vs currencies
- **get_trending**: Get trending search coins
- **list_asset_platforms**: List all asset platforms
- **get_coin_history**: Get historical data at a given date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinGecko** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of Bitcoin and Solana in USD?"

**🤖 AI Agent:**
> I've checked the latest data: Bitcoin is currently trading at $64,230.12 and Solana is at $145.67 USD. Both have seen a slight increase in the last 24 hours.

---

**👤 You:**
> "Show me the top 5 coins by market cap in the 'decentralized-finance-defi' category."

**🤖 AI Agent:**
> Fetching DeFi market leaders... The top 5 are: 1. Lido Staked Ether (STETH), 2. Dai (DAI), 3. Uniswap (UNI), 4. Chainlink (LINK), and 5. Wrapped BTC (WBTC).

---

**👤 You:**
> "Get the global cryptocurrency market statistics."

**🤖 AI Agent:**
> The total crypto market cap is approximately $2.45 trillion, with a 24h volume of $85 billion. Bitcoin dominance stands at 52.1% and Ethereum at 16.8%.


## ❓ FAQ

**Q: How can I check the current price of multiple cryptocurrencies at once?**
You can use the `get_simple_price` tool. Just provide a comma-separated list of IDs (e.g., 'bitcoin,ethereum,solana') and the target currency (e.g., 'usd') to get instant valuations.

**Q: Can the AI identify which coins are currently trending in the market?**
Yes! By using the `get_trending` tool, your agent will retrieve the top-7 trending coins on CoinGecko as searched by users in the last 24 hours.

**Q: Is it possible to get detailed information about a specific token's contract on a network?**
Absolutely. Use the `get_onchain_token` tool with the network ID and contract address to fetch precise on-chain data, including pool information and token metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coingecko-alternative](https://vinkius.com/mcp/coingecko-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinGecko** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coingecko-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinGecko** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coingecko-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
