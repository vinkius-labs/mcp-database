# Inside Bar Breakout Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inside-bar-breakout-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Detect volatility contraction and explosive breakouts using inside bar patterns.

## Description
This MCP server provides deterministic tools to identify volatility contraction through inside bar patterns. It identifies periods where price range tightens, signaling a potential explosive move. Use `analyze_patterns` to find contraction metrics, `detect_signals` to identify high-conviction breakouts with volume confirmation, and `get_trade_metrics` to evaluate strategy performance.


## Available Tools (3)
- **analyze_patterns**: Identify inside bar formations and calculate contraction metrics
- **detect_signals**: Identify valid buy and sell entry signals based on breakout rules
- **get_trade_metrics**: Provide statistical summary of the strategy performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inside Bar Breakout Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these price arrays for inside bar patterns: highs=[10, 12, 11], lows=[5, 6, 7], closes=[8, 11, 9], volumes=[100, 80, 90]"

**🤖 AI Agent:**
> The analysis identified an inside bar at index 2 with a compression ratio of 0.41.

---

**👤 You:**
> "Detect breakout signals for the following data: highs=[10, 12, 11, 13], lows=[5, 6, 7, 4], volumes=[100, 80, 90, 200], avgVolume=100, atr=[1, 1, 1, 1]"

**🤖 AI Agent:**
> A BUY signal was detected at bar index 3 with an entry price of 13.0.

---

**👤 You:**
> "Calculate the performance metrics for these signals: signals=[{barIndex: 1, side: 'BUY', entryPrice: 10, stopLoss: 9, takeProfit: 12}], priceHistory=[10, 11, 12, 9]"

**🤖 AI Agent:**
> The strategy achieved a win rate of 100% with a total profit of 2.0.


## ❓ FAQ

**Q: How does the strategy identify a breakout?**
A breakout is confirmed when the price breaches the high or low of the inside bar with volume exceeding 1.5x the average volume.

**Q: What is the purpose of the compression ratio?**
The compression ratio measures how much the price range has tightened compared to the previous bar, helping to identify high-potential setups.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inside-bar-breakout-strategy](https://vinkius.com/mcp/inside-bar-breakout-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inside Bar Breakout Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inside-bar-breakout-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inside Bar Breakout Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inside-bar-breakout-strategy": {
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
