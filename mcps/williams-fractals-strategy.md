# Williams Fractals Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/williams-fractals-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify price reversals and breakout signals using deterministic Williams Fractals.

## Description
This MCP server provides tools to identify price extrema and execute breakout strategies using Williams Fractals. It allows AI agents to analyze price series for Up-Fractals and Down-Fractals, calculate fractal density and amplitude, and generate validated BUY, SELL, or HOLD signals. By using `analyze_fractal_patterns`, agents can detect structural metrics, while `evaluate_trading_signals` provides entry prices, stop-losses, and take-profit levels based on volatility-adjusted rules. The `get_market_regime_context` tool helps determine trend strength and volatility levels.


## Available Tools (3)
- **analyze_fractal_patterns**: Identify confirmed Up and Down fractals and calculate structural metrics
- **evaluate_trading_signals**: Determine Buy, Sell, or Hold signals based on current price and fractal data
- **get_market_regime_context**: Provide a summary of recent fractal activity to understand market structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Williams Fractals Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these high and low prices for fractal patterns: [10, 12, 15, 13, 11, 10, 12, 14, 16, 14, 12]"

**🤖 AI Agent:**
> The analysis identified an Up-Fractal at index 2 with a price of 15 and a Down-Fractal at index 5 with a price of 10. The current fractal density is 2 in the last 20 bars.

---

**👤 You:**
> "Should I buy if the current price is 16, the last fractal was an Up-Fractal at 15, and the ATR is 1?"

**🤖 AI Agent:**
> BUY signal: Entry Price: 16.0, Stop-Loss: 14.0, Take-Profit: 18.0.

---

**👤 You:**
> "What is the current market regime based on this fractal data: {"density": 5, "trendStrength": "Bullish", "lastFractalType": "UP_FRACTAL"}?"

**🤖 AI Agent:**
> The market is in a High Volatility regime with Bullish trend strength.


## ❓ FAQ

**Q: How are fractals confirmed?**
A fractal is confirmed two bars after the middle bar (the peak or trough) satisfies the extremum condition.

**Q: What triggers a BUY signal?**
A BUY signal is triggered when the current price breaks above the most recent Up-Fractal, provided the last confirmed fractal was an Up-Fractal.

**Q: How is risk managed in this strategy?**
Stop-loss levels are set using the opposite fractal price or a 2x ATR adjustment, while take-profit targets use the next fractal level or a 3:1 reward-to-risk ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/williams-fractals-strategy](https://vinkius.com/ai-agent-connect/williams-fractals-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Williams Fractals Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `williams-fractals-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Williams Fractals Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "williams-fractals-strategy": {
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
