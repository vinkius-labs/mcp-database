# Elder-Ray Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/elder-ray-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic trading signals using Bulls and Bears Power indicators.

## Description
This MCP server provides deterministic trading signals based on the Elder-Ray Index. It uses `calculate_elder_ray_metrics` to compute Bulls Power, Bears Power, and Market Force. By analyzing these metrics alongside EMA trends, the `generate_trading_signals` tool identifies precise BUY and SELL entries. You can also use `analyze_market_regime` to determine if the market is in Trend Dominance, Equilibrium, or a Reversal Zone.


## Available Tools (3)
- **analyze_market_regime**: Provide a high-level summary of the current market state
- **calculate_elder_ray_metrics**: Compute fundamental Elder-Ray indicators and market force
- **generate_trading_signals**: Evaluate price action and indicator trends to produce BUY, SELL, or HOLD signals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elder-Ray Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Elder-Ray metrics for this price data: [{'high': 150, 'low': 145, 'close': 148}, {'high': 155, 'low': 148, 'close': 152}]"

**🤖 AI Agent:**
> { "bullsPower": [2, 7], "bearsPower": [-3, -3], "marketForce": [5, 10], "emaSlope": [0.5, 1.2], "emaValues": [146, 147.5] }

---

**👤 You:**
> "Generate trading signals based on these metrics and price data."

**🤖 AI Agent:**
> { "signals": [{ "timestamp": "2023-10-27T10:00:00Z", "type": "BUY", "entryPrice": 152.0, "stopLoss": 148.5, "takeProfit": 161.5 }] }

---

**👤 You:**
> "What is the current market regime for these power values?"

**🤖 AI Agent:**
> { "regimeStatus": "Trend Dominance", "bullishStrength": 12.5, "bearishStrength": 2.1 }


## ❓ FAQ

**Q: What indicators does this strategy use?**
It uses the Elder-Ray Index, specifically Bulls Power, Bears Power, and the Exponential Moving Average (EMA).

**Q: How are BUY signals generated?**
A BUY signal is triggered when Bulls Power is positive, Bears Power is negative but rising, and the price is above the EMA, provided Bulls Power has been rising for at least two bars.

**Q: Can I analyze market volatility?**
Yes, by using `analyze_market_regime`, you can identify if the market is in a Trend Dominance, Equilibrium, or Reversal Zone.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/elder-ray-strategy](https://vinkius.com/ai-agent-connect/elder-ray-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Elder-Ray Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `elder-ray-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Elder-Ray Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "elder-ray-strategy": {
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
