# Trend-Following Ensemble Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/trend-following-ensemble-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generates high-conviction trade signals using an ensemble of MA, MACD, and ADX indicators.

## Description
This MCP server provides a deterministic technical analysis engine that aggregates multiple trend signals into a unified ensemble score. By requiring unanimous agreement between Moving Average crossovers, MACD momentum, and ADX trend strength, it filters out market noise and identifies high-conviction entries. Use `analyze_trend_ensemble` to generate complete trade signals including entry prices, stop-loss, and take-profit levels. You can also use `calculate_momentum_health` to assess trend acceleration and `evaluate_risk_parameters` to manage exits based on volatility.


## Available Tools (3)
- **analyze_trend_ensemble**: Executes the core logic to generate trade signals and ensemble metrics based on price data
- **calculate_momentum_health**: Evaluates the specific momentum components to determine if a trend is accelerating or decelerating
- **evaluate_risk_parameters**: Determines the price levels for exiting a trade based on current volatility and price action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trend-Following Ensemble Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the trend for these closing prices: [150.2, 152.5, 155.0, 154.8, 158.2, 160.5, 162.0]"

**🤖 AI Agent:**
> The current ensemble score is 3, indicating a strong BUY signal with an entry price of 162.0, a stop-loss of 158.2, and a take-profit of 173.4.

---

**👤 You:**
> "Check the momentum health for these MACD and signal values: MACD=[0.5, 0.6, 0.7], Signal=[0.1, 0.2, 0.3], Zero=0"

**🤖 AI Agent:**
> The momentum is bullish with a strength of 0.7.

---

**👤 You:**
> "Calculate risk parameters for a BUY trade at 100 with a swing low of 95, ATR of 2, and a multiplier of 2."

**🤖 AI Agent:**
> The stop-loss is 95.0 and the take-profit is 111.0.


## ❓ FAQ

**Q: What is an ensemble score?**
The ensemble score is a count of how many independent technical signals (MA, MACD, and ADX) align. A score of 3 indicates unanimous agreement, which triggers a high-conviction trade signal.

**Q: How are stop-loss and take-profit levels determined?**
Exit levels are calculated using `evaluate_risk_parameters`, which uses recent price swings and the Average True Range (ATR) to set protective stops and target a 3:1 reward-to-risk ratio.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/trend-following-ensemble-strategy](https://vinkius.com/ai-agent-connect/trend-following-ensemble-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trend-Following Ensemble Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trend-following-ensemble-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trend-Following Ensemble Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trend-following-ensemble-strategy": {
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
