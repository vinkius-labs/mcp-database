# Scalping Strategy Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scalping-strategy-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic momentum-based scalping engine using EMA and Stochastic oscillators.

## Description
This MCP server provides a deterministic engine for high-probability scalping. It identifies trend-following momentum reversals by combining Exponential Moving Averages (EMA) with Stochastic oscillators. The engine uses `calculate_signals` to detect precise entry points where price trends align with momentum exhaustion. Users can further refine their analysis using `evaluate_scalp_quality` to assess trade strength via price-to-EMA distance and Stochastic slope, or use `get_market_filters` to ensure liquidity and low transaction costs before entering a position.


## Available Tools (3)
- **get_market_filters**: Validates if current market conditions (liquidity and cost) permit scalping
- **calculate_signals**: Generates precise buy, sell, or hold signals for a historical price series based on trend and momentum criteria
- **evaluate_scalp_quality**: Analyzes a specific signal to provide a granular assessment of the trade's strength


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scalping Strategy Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate scalping signals for this price data: [{"close": 150.5, "high": 151.0, "low": 149.5, "volume": 1000, "bid": 150.4, "ask": 150.6}]"

**🤖 AI Agent:**
> {"timestamp": "2023-10-27T10:00:00Z", "signal": "BUY", "entryPrice": 150.5, "stopLoss": 150.25, "takeProfit": 151.12, "scalpQuality": 0.85}

---

**👤 You:**
> "Check the quality of a signal where price is 150, EMA is 148, stochK is 15, stochD is 10, and previousStochK was 12."

**🤖 AI Agent:**
> {"distanceFromEmaRatio": 0.0135, "stochSlope": 0.25}

---

**👤 You:**
> "Are current market conditions suitable for scalping with this data: [{"volume": 500, "bid": 100.0, "ask": 100.01}] and an average volume window of 10?"

**🤖 AI Agent:**
> {"isLiquid": false, "isLowCost": true}


## ❓ FAQ

**Q: What indicators does this engine use?**
The engine uses Exponential Moving Averages (EMA) for trend direction and Stochastic oscillators (%K and %D) for momentum identification.

**Q: How is the scalp quality determined?**
Quality is determined by the relative distance between the price and the EMA, alongside the slope of the Stochastic %K line.

**Q: Does it filter for liquidity?**
Yes, the engine includes filters to ensure volume is above average and the bid-ask spread remains within a low-cost threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scalping-strategy-engine](https://vinkius.com/mcp/scalping-strategy-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scalping Strategy Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scalping-strategy-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scalping Strategy Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scalping-strategy-engine": {
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
