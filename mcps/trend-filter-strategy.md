# Trend Filter Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/trend-filter-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic trading strategy using ADX for trend detection and Moving Averages for execution.

## Description
This MCP server provides a deterministic framework for identifying market regimes and executing trades. By using `analyze_trend_regime`, agents can distinguish between Uptrend, Downtrend, and Sideways markets based on ADX strength and Moving Average positioning. Once a regime is identified, `calculate_trading_signals` generates precise entry, stop-loss, and take-profit instructions based on price pullbacks. Additionally, `get_trend_metrics` provides quantitative data on trend strength and momentum to assist in decision making.


## Available Tools (3)
- **analyze_trend_regime**: Determines the current market state (Uptrend, Downtrend, or Sideways) based on ADX and Moving Average positioning
- **calculate_trading_signals**: Identifies specific Buy or Sell signals based on the current trend regime and price action
- **get_trend_metrics**: Provides quantitative data regarding the current strength and momentum of the trend


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trend Filter Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current market regime for these closing prices: [150.2, 151.5, 152.0, 149.5, 148.0, 153.0, 155.0]"

**🤖 AI Agent:**
> The current market regime is UPTREND with an ADX value of 28.5 and a positive MA slope.

---

**👤 You:**
> "Generate a trading signal for an uptrend where the price has just touched the 50 EMA."

**🤖 AI Agent:**
> BUY signal generated: Entry Price 150.00, Stop-Loss 147.50, Take-Profit 157.50.

---

**👤 You:**
> "What is the current trend strength and momentum?"

**🤖 AI Agent:**
> The current trend strength is 0.75 and the momentum score is 12.4.


## ❓ FAQ

**Q: How does the strategy determine the market regime?**
The regime is determined by the ADX value and the price position relative to the Moving Average. An Uptrend is identified when ADX is above 25 and price is above the MA.

**Q: What kind of signals does this MCP provide?**
It provides BUY and SELL signals based on pullbacks to the Moving Average during trending regimes, as calculated by `calculate_trading_signals`.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/trend-filter-strategy](https://vinkius.com/ai-agent-connect/trend-filter-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trend Filter Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trend-filter-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trend Filter Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trend-filter-strategy": {
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
