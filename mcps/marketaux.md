# Marketaux MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketaux)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Financial news and stock market intelligence — track global market sentiment and trending news.

## Description
Connect your **Marketaux** account to any AI agent and stay on top of the financial markets through natural conversation.

### What you can do

- **Financial News** — Search global news by symbol, keyword, or language
- **Sentiment Analysis** — Filter news by market sentiment to understand impacts
- **Market Data** — Query symbols, entities, exchanges, and industries
- **Live Status** — Check stock market status and global indices

### How it works

1. Subscribe to this server
2. Enter your Marketaux API Token
3. Start querying financial intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_entities**: ) tracked by Marketaux.

Get entity data
- **get_indices**: List stock indices
- **get_latest_news**: Get the latest financial news
- **get_sentiment_analysis**: Get news with sentiment analysis
- **get_stock_market_status**: Get stock market status
- **get_symbols**: List supported stock symbols
- **get_trending_news**: Get trending financial news
- **list_industries**: List industries
- **search_exchanges**: Search for stock exchanges
- **search_news**: Search for global financial news


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketaux** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show latest news for AAPL and MSFT."

**🤖 AI Agent:**
> Fetching latest news... I found articles regarding Apple's latest earnings and Microsoft's new AI features.

---

**👤 You:**
> "Check if the stock market is open now."

**🤖 AI Agent:**
> Market status query... Global markets like NYSE and NASDAQ are currently open.

---

**👤 You:**
> "What are the trending financial topics today?"

**🤖 AI Agent:**
> Retrieving trending news... Today's focus is on inflation reports and energy sector shifts.


## ❓ FAQ

**Q: How do I find my Marketaux API Token?**
Log in to your Marketaux account and navigate to the Dashboard to see your API Token.

**Q: What stock symbols are supported?**
Marketaux supports most major global stock symbols. You can use the `get_symbols` tool to search for specific ones.

**Q: Is the sentiment analysis accurate?**
Marketaux uses advanced AI to score news sentiment. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketaux](https://vinkius.com/mcp/marketaux)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marketaux** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `marketaux` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marketaux** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketaux": {
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
