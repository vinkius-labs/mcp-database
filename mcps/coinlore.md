# CoinLore MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coinlore)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time cryptocurrency data, market stats, exchange info, and social metrics directly from any AI agent.

## Description
Connect to the **CoinLore** API to empower your AI agent with comprehensive cryptocurrency market intelligence and real-time blockchain data.

### What you can do

- **Market Overview** — Get global cryptocurrency statistics including total market cap, volume, and BTC/ETH dominance.
- **Ticker Data** — Retrieve detailed price, volume, and supply data for thousands of coins using specific IDs.
- **Market Movers** — Instantly identify the top 20 gainers and losers across different timeframes (1h, 24h, 7d).
- **Historical Analysis** — Access 365 days of daily OHLCV (Open, High, Low, Close, Volume) history for deep trend analysis.
- **Exchange Intelligence** — List all supported exchanges and inspect specific trading pairs and top 100 markets.
- **Social Sentiment** — Monitor social media metrics from Twitter and Reddit to gauge community engagement for specific assets.

### How it works

1. Subscribe to this server
2. No API key is required for the public tier; simply initialize the connection
3. Start querying crypto markets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Traders & Investors** — Quickly check market movers and coin-specific metrics without switching to a browser.
- **Data Analysts** — Fetch historical OHLCV data and global stats directly into your analysis environment.
- **Developers** — Integrate crypto pricing and metadata into your workflow using natural language commands.


## Available Tools (11)
- **get_global_stats**: Get overall cryptocurrency market statistics
- **get_movers**: Get top 20 winners and losers
- **get_ohlcv**: Get 365 days of daily OHLCV history
- **get_social_stats**: Get social media metrics for a coin
- **get_ticker**: Retrieve detailed tick data for specific coins
- **list_tickers**: Retrieve tick data for multiple coins
- **list_assets**: Get a lightweight list of all coins
- **get_coin_info**: Get static metadata for a specific coin
- **get_coin_markets**: Get top 50 exchanges and markets for a coin
- **get_exchange**: Get exchange details and top 100 trading pairs
- **list_exchanges**: Get all exchanges listed on CoinLore


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinLore** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current global crypto market cap and BTC dominance?"

**🤖 AI Agent:**
> I've retrieved the global stats: The total market cap is approximately $2.45 trillion with a 24h volume of $85 billion. Bitcoin dominance currently stands at 52.1%.

---

**👤 You:**
> "Show me the top 20 gainers in the last 24 hours."

**🤖 AI Agent:**
> Fetching market movers... The top gainer is 'CoinX' with a 24.5% increase, followed by 'TokenY' at 18.2%. Would you like more details on any of these?

---

**👤 You:**
> "Get the price and social stats for Ethereum (ID: 80)."

**🤖 AI Agent:**
> Ethereum (ETH) is currently trading at $3,450. On the social side, it has over 3 million Twitter followers and high engagement on Reddit today.


## ❓ FAQ

**Q: How can I see which cryptocurrencies are performing best today?**
You can use the `get_movers` tool. It retrieves the top 20 gainers and losers in the market based on your preferred timeframe (1h, 24h, or 7d).

**Q: Is it possible to get historical price data for a specific coin?**
Yes! The `get_ohlcv` tool provides 365 days of daily Open, High, Low, Close, and Volume history for any coin using its CoinLore ID.

**Q: Can I check the social media popularity of a cryptocurrency?**
Absolutely. Use the `get_social_stats` tool with a coin's ID to retrieve metrics from Twitter and Reddit, including follower counts and engagement stats.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinlore](https://vinkius.com/mcp/coinlore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinLore** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coinlore` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinLore** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coinlore": {
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
