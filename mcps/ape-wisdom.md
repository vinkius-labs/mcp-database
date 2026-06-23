# Ape Wisdom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ape-wisdom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Track trending stocks and cryptocurrencies based on social media sentiment from Reddit and 4chan.

## Description
The **Ape Wisdom MCP Server** allows your AI agent to tap into the pulse of retail investors. By monitoring mentions and sentiment on popular boards like r/wallstreetbets, r/CryptoCurrency, and 4chan, this server provides real-time insights into what the internet is talking about in the financial and crypto markets.

### What you can do

- **Trending Assets** — List the most mentioned stocks and coins across all major subreddits.
- **Sentiment Analysis** — Check whether the social conversation around a specific ticker is positive or negative.
- **Mention Growth** — Identify 'top gainers' in terms of social media buzz to spot emerging trends before they hit the mainstream.
- **Board-Specific Filtering** — Narrow down results to specific communities like WallStreetBets or general crypto boards.
- **Market Snapshot** — Get a high-level summary of the top trending assets in both the stock and crypto categories.

### How it works

1. Subscribe to this server
2. No API Key required (Public API)
3. Start querying social sentiment data through your AI chat interface.

### Who is this for?

- **Traders** — Spot trending assets and gauge retail sentiment to inform your trading strategy.
- **Market Researchers** — Track how social buzz correlates with market movements.
- **Social Media Managers** — Monitor the conversation around specific brands or assets in the crypto space.


## Available Tools (10)
- **get_market_snapshot**: Get a quick summary of top trending stocks and crypto
- **get_sentiment_leaders**: Get assets with the highest positive sentiment
- **get_top_gainers**: Get assets with the highest mention growth in the last 24h
- **list_all_trending**: List trending stocks and crypto from all boards
- **list_trending_4chan**: List trending assets from 4chan boards
- **list_trending_crypto**: List trending cryptocurrencies from crypto-focused subreddits
- **list_trending_stocks**: List trending stocks from stock-focused subreddits
- **list_trending_subreddit**: List trending assets from a specific subreddit
- **list_wallstreetbets**: List trending assets specifically from r/wallstreetbets
- **search_ticker**: Search for a specific ticker or coin in the trending lists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ape Wisdom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the top 10 trending stocks on Reddit right now?"

**🤖 AI Agent:**
> I've pulled the latest trending stocks. Currently, NVDA leads with 1,250 mentions, followed by TSLA and AAPL. The sentiment for NVDA is strongly positive at 0.78.

---

**👤 You:**
> "Show me cryptocurrencies with the highest mention growth in the last 24 hours."

**🤖 AI Agent:**
> The top gainers in social buzz are SOL (+450 mentions), PEPE (+320 mentions), and ETH (+280 mentions). SOL is seeing a significant spike in r/CryptoCurrency.

---

**👤 You:**
> "Get a market snapshot of trending assets."

**🤖 AI Agent:**
> Here's your market snapshot. For stocks, NVDA and AMD are dominating the conversation. For crypto, BTC and ETH remain at the top, with a surge in interest for modular blockchains.


## ❓ FAQ

**Q: Is an API key required for Ape Wisdom?**
No, this server uses Ape Wisdom's public API v1.0, which does not require authentication for basic usage.

**Q: Which social platforms are tracked?**
Ape Wisdom primarily tracks popular investment-related subreddits on Reddit (like r/wallstreetbets, r/stocks, r/CryptoCurrency) and the /biz/ board on 4chan.

**Q: What does the sentiment value represent?**
The sentiment value indicates the general tone of the social conversation. Values closer to 1.0 indicate highly positive sentiment, while lower values suggest negative or cautious conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ape-wisdom](https://vinkius.com/mcp/ape-wisdom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ape Wisdom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ape-wisdom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ape Wisdom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ape-wisdom": {
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
