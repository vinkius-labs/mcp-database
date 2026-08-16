# Breakout Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/breakout-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic Donchian Channel breakout strategy based on Turtle Trader principles.

## Description
This MCP server provides quantitative tools to execute a trend-following strategy using Donchian Channels. It identifies price breakouts by monitoring high and low price ranges, filtered by ADX trend strength and volume confirmation. Use `calculate_signals` to identify entry and exit points, `get_summary_statistics` to analyze performance metrics like max drawdown, and `validate_market_conditions` to check if the market is in a Trending, Ranging, or Exhaustion tier.


## Available Tools (3)
- **calculate_signals**: Analyzes historical price and volume data to generate specific buy, sell, or hold signals for every time interval (bar)
- **get_summary_statistics**: Provides a high-level overview of the strategy's performance and market conditions over a specific range
- **validate_market_conditions**: Checks if the current market environment is suitable for the breakout strategy based on trend and volatility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breakout Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate buy signals for this price data."

**🤖 AI Agent:**
> The system identified a BUY signal at bar 25 with an entry price of 150.50 and a stop-loss of 145.20.

---

**👤 You:**
> "Is the current market trending?"

**🤖 AI Agent:**
> Yes, the ADX is 30, which indicates a trending market.

---

**👤 You:**
> "What are the summary statistics for this dataset?"

**🤖 AI Agent:**
> The average volatility was 2.5, with a maximum drawdown of 12% and 5 total buy signals.


## ❓ FAQ

**Q: How are buy signals generated?**
A BUY signal is triggered when the price closes above the highest high of the preceding entry period, provided volume is high and ADX indicates a strong trend.

**Q: What is the purpose of the `validate_market_conditions` tool?**
It checks if the current market environment is suitable for trading by evaluating trend strength, volume, and price exhaustion.

**Q: How is position size determined?**
Position size is calculated using ATR to risk exactly 1% of total capital per trade.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/breakout-strategy](https://vinkius.com/ai-agent-connect/breakout-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breakout Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breakout-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breakout Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breakout-strategy": {
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
