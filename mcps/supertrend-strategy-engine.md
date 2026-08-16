# SuperTrend Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/supertrend-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic trend-following strategy with volatility and trend-strength filters.

## Description
This MCP server provides a deterministic engine for executing the SuperTrend trend-following strategy. It uses volatility-based indicators to identify market direction and provides precise entry and exit signals. The engine includes built-in filters to ensure high-quality trades: it requires a minimum trend strength via ADX and avoids low-volatility environments by comparing current ATR against recent historical lows. Use `get_trend_signals` to identify BUY and SELL entries, `get_trend_metrics` for real-time trend statistics like slope and duration, and `get_volatility_status` to assess market movement requirements.


## Available Tools (3)
- **get_trend_metrics**: Provides detailed statistical context regarding the current trend
- **get_trend_signals**: Calculates SuperTrend signals and filters
- **get_volatility_status**: Analyzes recent volatility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SuperTrend Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the latest trend signals for these prices."

**🤖 AI Agent:**
> The latest signal is a BUY at price 150.25 with a stop-loss at 148.50.

---

**👤 You:**
> "Is the current market volatility too low to trade?"

**🤖 AI Agent:**
> No, the current ATR is 15.4, which is above the 10-day low of 12.1.

---

**👤 You:**
> "What are the current trend metrics?"

**🤖 AI Agent:**
> The current trend is bullish with a duration of 12 bars and a positive slope.


## ❓ FAQ

**Q: How are BUY signals generated?**
A BUY signal is triggered when the price closes above the SuperTrend line and the ADX value is greater than 20, ensuring the trend is strong enough to trade.

**Q: What is the purpose of the volatility filter?**
The volatility filter prevents trading in 'choppy' or sideways markets by checking if the current ATR is lower than the minimum ATR observed over the last 10 days.

**Q: How does the stop-loss work?**
The SuperTrend line itself acts as a dynamic trailing stop-loss, automatically adjusting as the trend evolves.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/supertrend-strategy-engine](https://vinkius.com/ai-agent-connect/supertrend-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SuperTrend Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supertrend-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SuperTrend Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supertrend-strategy-engine": {
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
