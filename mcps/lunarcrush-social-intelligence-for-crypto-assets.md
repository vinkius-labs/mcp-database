# LunarCrush (Social Intelligence for Crypto Assets) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lunarcrush-social-intelligence-for-crypto-assets)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access real-time social intelligence for crypto assets — track Galaxy Scores, AltRank, and market sentiment directly from your AI agent.

## Description
Connect **LunarCrush** to any AI agent to unlock deep social insights for the crypto market. This server allows you to monitor community sentiment, social engagement, and proprietary metrics like Galaxy Score and AltRank for thousands of digital assets.

### What you can do

- **Asset Discovery** — List all supported crypto assets and filter by symbol or rank using `list_assets`.
- **Galaxy Score** — Get a combined measure of social and market performance relative to historical data via `get_galaxy_score`.
- **AltRank** — Measure a coin's social performance relative to the entire crypto market using `get_altrank`.
- **Social Intelligence** — Fetch detailed engagement, mentions, and sentiment metrics with `get_social_metrics`.
- **Market Data** — Access real-time price, volume, and market cap information through `get_market_metrics`.

### How it works

1. Subscribe to this server
2. Enter your LunarCrush API Key
3. Start analyzing crypto trends from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Crypto Traders** — identify trending assets based on social volume and sentiment shifts
- **Analysts** — combine social intelligence with market metrics for deeper research
- **Developers** — integrate crypto social data into automated workflows and agents


## Available Tools
- **get_altrank**: Get AltRank for a specific coin
- **list_assets**: Can be filtered by symbol, sorted, and limited.

Retrieve a list of all supported assets or specific details
- **get_galaxy_score**: Get Galaxy Score for a specific coin
- **get_market_metrics**: Get market metrics for a coin
- **get_social_metrics**: Get detailed social metrics for a coin


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LunarCrush (Social Intelligence for Crypto Assets)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top 10 crypto assets sorted by Galaxy Score."

**🤖 AI Agent:**
> I've retrieved the top assets. Currently, Bitcoin (BTC) leads with a Galaxy Score of 78, followed by Ethereum (ETH) at 74. Would you like to see the social metrics for any of these?

---

**👤 You:**
> "What is the current AltRank for Solana (SOL)?"

**🤖 AI Agent:**
> Solana (SOL) currently has an AltRank of 12. This indicates very strong social performance relative to the rest of the market. Its social engagement has increased by 15% in the last 24 hours.

---

**👤 You:**
> "Show me social engagement and sentiment for BTC over the last 24 hours."

**🤖 AI Agent:**
> For Bitcoin (BTC) in the last 24h: Social mentions are at 120k, engagement is up 5%, and the overall sentiment remains 'Bullish' at 72%.


## ❓ FAQ

**Q: What does the Galaxy Score represent for a coin?**
The Galaxy Score, retrieved via `get_galaxy_score`, indicates how a coin is performing relative to its own historical social and market performance. A higher score suggests stronger combined health.

**Q: How can I compare a coin's social performance against the entire market?**
Use the `get_altrank` tool. It measures a coin's social performance relative to the entire crypto market, helping you identify assets that are gaining significant social traction.

**Q: Can I get social sentiment for specific time intervals?**
Yes! The `get_social_metrics` tool allows you to specify an interval (1h, 24h, or 7d) to retrieve mentions, engagement, and sentiment for a specific coin symbol.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lunarcrush-social-intelligence-for-crypto-assets](https://vinkius.com/mcp/lunarcrush-social-intelligence-for-crypto-assets)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LunarCrush (Social Intelligence for Crypto Assets)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lunarcrush-social-intelligence-for-crypto-assets` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LunarCrush (Social Intelligence for Crypto Assets)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lunarcrush-social-intelligence-for-crypto-assets": {
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
