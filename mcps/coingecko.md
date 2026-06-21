# CoinGecko MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coingecko)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Enable your AI agent to query crypto prices, market rankings, and global market stats via the CoinGecko API.

## Description
Connect your AI to **CoinGecko**, the crypto market data platform tracking price, volume, market cap, community growth, and open-source development.

### What you can do

- **Price Queries** — Get the current price of any cryptocurrency in multiple fiat currencies.
- **Market Rankings** — List the top coins by market cap, volume, or price change.
- **Global Stats** — Retrieve aggregate market data including total market cap, 24h volume, and BTC dominance.

### How it works

1. Add the CoinGecko integration to your AI toolset.
2. Provide your API Key (Demo or Pro, from coingecko.com).
3. Query crypto market data via natural language.

### Who is this for?

- **Crypto Traders** — Get live prices and market rankings from chat.
- **Analysts** — Pull fundamental market data for research and reports.
- **Developers** — Integrate crypto pricing into automated workflows.


## Available Tools
- **get_coin_details**: Retrieve detailed information about a specific cryptocurrency
- **get_global_data**: Retrieve global cryptocurrency market data
- **get_price**: Retrieve the current price of one or more cryptocurrencies
- **get_trending**: Retrieve trending coins from the last 24 hours
- **list_categories**: Retrieve a list of all cryptocurrency categories
- **list_exchanges**: Retrieve a list of cryptocurrency exchanges
- **list_markets**: Retrieve a list of coins with detailed market data
- **search_crypto**: Search for coins, exchanges, and categories by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinGecko** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current price of Bitcoin in USD and BRL?"

**🤖 AI Agent:**
> Bitcoin (BTC):
- USD: $67,420.00 (+2.3% 24h)
- BRL: R$ 337,100.00 (+2.5% 24h)
Market cap: $1.32T | 24h volume: $28.4B

---

**👤 You:**
> "Show me the global cryptocurrency market stats."

**🤖 AI Agent:**
> Global Crypto Market:
- Total Market Cap: $2.54T (+1.8% 24h)
- 24h Volume: $98.2B
- BTC Dominance: 52.1%
- ETH Dominance: 16.3%
- Active Cryptocurrencies: 14,200+
Want a breakdown by category (DeFi, NFT, etc.)?

---

**👤 You:**
> "List the top 5 trending coins on CoinGecko right now."

**🤖 AI Agent:**
> The top 5 trending coins in the last 24h are: 1. Solana (SOL) 2. Jupiter (JUP) 3. Pepe (PEPE) 4. Fetch.ai (FET) 5. Render (RNDR).


## ❓ FAQ

**Q: Do I need an API key?**
Yes. CoinGecko requires an API key for all v3 endpoints. You can get a free Demo key on their website.

**Q: What is the difference between Demo and Pro keys?**
Demo keys have lower rate limits and use the public API URL. Pro keys have higher limits and use a dedicated Pro API URL.

**Q: How often is the data updated?**
On the free tier, data is typically updated every 60 seconds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coingecko](https://vinkius.com/mcp/coingecko)
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
3. Set Type to "SSE", enter `coingecko` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinGecko** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coingecko": {
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
