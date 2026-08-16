# Golden Cross Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/golden-cross-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic trend-following engine for Golden Cross and Death Cross signals.

## Description
This MCP server provides a deterministic execution engine for identifying market trends using moving average crossovers. It identifies Golden Cross and Death Cross events, calculates signal strength, and generates precise trade execution plans including entry prices, stop-loss, and take-profit levels. Use `calculate_cross_signals` to find historical crossovers, `generate_trade_execution` to define risk parameters, and `analyze_strategy_performance` to evaluate historical win rates.


## Available Tools (3)
- **analyze_strategy_performance**: Evaluate the historical effectiveness of the strategy based on past signals and trades
- **calculate_cross_signals**: Identify all historical Golden Cross and Death Cross events within a price series
- **generate_trade_execution**: Calculate specific entry, exit, and risk parameters for a confirmed signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Golden Cross Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all Golden Cross signals in this price data: [150, 152, 155, 158, 160, 162, 165]"

**🤖 AI Agent:**
> The signal was detected at the price point where the fast MA crossed the slow MA.

---

**👤 You:**
> "Calculate a trade plan for a signal at price 100 with an ATR of 5 and a 3:1 reward-risk ratio."

**🤖 AI Agent:**
> The entry price is 100, the stop-loss is 95, and the take-profit is 115.

---

**👤 You:**
> "What was the win rate for these 10 signals and 5 trades?"

**🤖 AI Agent:**
> The historical win rate for the provided data is 60%.


## ❓ FAQ

**Q: What is a Golden Cross?**
A Golden Cross occurs when a fast moving average crosses above a slow moving average, signaling a bullish trend.

**Q: How do I calculate my risk parameters?**
You can use the `generate_trade_execution` tool to automatically calculate entry, stop-loss, and take-profit based on ATR and reward-risk ratios.

**Q: Can I use SMA or EMA?**
Yes, the engine supports both Simple Moving Averages (SMA) and Exponential Moving Averages (EMA).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/golden-cross-strategy-engine](https://vinkius.com/ai-agent-connect/golden-cross-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Golden Cross Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `golden-cross-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Golden Cross Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "golden-cross-strategy-engine": {
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
