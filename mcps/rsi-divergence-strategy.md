# RSI Divergence Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/rsi-divergence-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify bullish and bearish RSI divergence signals for mean-reversion trading.

## Description
This MCP server provides deterministic tools to detect RSI divergences in price series. Use `calculate_rsi_divergence` to find BUY and SELL signals based on price extremes and RSI momentum shifts. You can also use `get_signal_summary` to analyze performance metrics or `identify_swing_points` to locate local price highs and lows. It is designed for traders looking to capture mean-reversion opportunities when momentum diverges from price action.


## Available Tools (3)
- **calculate_rsi_divergence**: 
- **identify_swing_points**: 
- **get_signal_summary**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RSI Divergence Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all divergence signals in this price data: [45.2, 44.8, 46.1, 43.5, 43.2, 44.5, 45.0]"

**🤖 AI Agent:**
> The strategy identified a BUY signal at bar index 5 with an entry price of 43.2 and a stop-loss at 43.0.

---

**👤 You:**
> "What was the average divergence strength for these signals?"

**🤖 AI Agent:**
> The average divergence strength for the provided signals is 12.5.

---

**👤 You:**
> "Identify the swing points for these prices: [10, 12, 11, 13, 12, 14, 13]"

**🤖 AI Agent:**
> The swing highs are at indices 1, 3, and 5, while the swing lows are at indices 0, 2, 4, and 6.


## ❓ FAQ

**Q: How are BUY signals generated?**
A BUY signal is triggered when a bullish divergence is confirmed: the price makes a lower low, but the RSI makes a higher low while below 30, followed by the RSI crossing back above 30.

**Q: What is the purpose of `get_signal_summary`?**
The `get_signal_summary` tool provides statistical insights including total signal counts, buy/sell ratios, and divergence strength metrics.

**Q: Can I customize the RSI period?**
Yes, the `calculate_rsi_divergence` tool allows you to specify a custom `rsiPeriod`, which defaults to 14.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/rsi-divergence-strategy](https://vinkius.com/ai-agent-connect/rsi-divergence-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RSI Divergence Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rsi-divergence-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RSI Divergence Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rsi-divergence-strategy": {
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
