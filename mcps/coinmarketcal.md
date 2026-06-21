# CoinMarketCal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coinmarketcal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [event-management](../categories/event-management.md)

Enable your AI agent to browse upcoming crypto events, listings, and forks via the CoinMarketCal API.

## Description
Connect your AI to **CoinMarketCal**, the leading economic calendar for the crypto market.

### What you can do

- **Event Search** — Find upcoming events for specific coins like Bitcoin, Ethereum, or any altcoin.
- **Trending Events** — List the most popular and community-voted events happening soon.
- **Category Filtering** — Filter by event type: exchange listings, hard forks, AMAs, conferences, roadmap milestones, and more.

### How it works

1. Add the CoinMarketCal integration to your AI toolset.
2. Provide your API Key (from developers.coinmarketcal.com).
3. Query upcoming crypto events via natural language.

### Who is this for?

- **Crypto Traders** — Stay ahead of market-moving events like listings and forks.
- **Analysts** — Track project milestones and conference dates for research.
- **Portfolio Managers** — Monitor events across held assets to anticipate volatility.


## Available Tools
- **get_coin_id**: Find the CoinMarketCal ID for a coin by its name or symbol
- **get_event_details**: Retrieve detailed information about a specific event by its ID
- **list_categories**: Retrieve the list of event categories (e.g., Roadmap, Release)
- **list_coins**: Retrieve the list of coins supported by CoinMarketCal
- **list_events**: Retrieve a list of cryptocurrency events from the calendar
- **list_popular_events**: Retrieve the most popular cryptocurrency events
- **list_trending_events**: Retrieve the most trending cryptocurrency events
- **search_events_by_coin**: Find events related to specific cryptocurrencies
- **search_events_by_date**: Find events within a specific date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoinMarketCal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me upcoming events for Bitcoin."

**🤖 AI Agent:**
> 3 upcoming Bitcoin events:
1. 'Lightning Network v2.0' — Apr 15 (Release, 92% confidence)
2. 'BTC Mining Conference' — Apr 22 (Conference, 87% confidence)
3. 'Taproot Upgrade Activation' — May 1 (Fork, 95% confidence)
Want details on any of these?

---

**👤 You:**
> "Show me upcoming exchange listings."

**🤖 AI Agent:**
> 5 upcoming exchange listings:
1. TOKEN-X on Binance — Apr 10 (98% confidence)
2. DEFI-Y on Coinbase — Apr 12 (85% confidence)
3. NFT-Z on Kraken — Apr 18 (72% confidence)
Want me to filter by a specific exchange?

---

**👤 You:**
> "List trending events happening this week."

**🤖 AI Agent:**
> The most trending events this week are: Ethereum's Network Upgrade (Thursday), Cardano's Africa Keynote (Friday), and the Binance Token Burn (Weekend). Check details for full coverage.


## ❓ FAQ

**Q: How do I get a CoinMarketCal API key?**
Apply for an API key at developers.coinmarketcal.com. Once approved, copy your key and paste it below.

**Q: Is the event information verified?**
CoinMarketCal uses a community-driven verification system. Each event has a confidence percentage and a proof link for validation.

**Q: What event categories are available?**
Categories include Roadmap, Release, Exchange Listing, AMA, Fork, Conference, Partnership, Airdrop, and more.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coinmarketcal](https://vinkius.com/mcp/coinmarketcal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CoinMarketCal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `coinmarketcal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CoinMarketCal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coinmarketcal": {
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
