# Intermarket Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/intermarket-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic mean-reversion engine for trading commodity ratio spreads.

## Description
This MCP server provides a deterministic engine for trading the relative value between highly correlated commodity futures. By utilizing ratio-based z-scores, the engine identifies mean-reversion opportunities when the relationship between two assets deviates significantly from historical norms. Users can use `analyze_spread_signals` to generate daily trading signals, `get_historical_context` to retrieve established bounds and economic drivers, and `validate_liquidity_thresholds` to ensure sufficient market participation for safe execution.


## Available Tools (3)
- **analyze_spread_signals**: 
- **get_historical_context**: get_historical_context
- **validate_liquidity_thresholds**: validate_liquidity_thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intermarket Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for a gold and silver spread using recent price and open interest data."

**🤖 AI Agent:**
> Asset A (Gold) Price: 2350.00, Asset B (Silver) Price: 28.50, Spread Ratio: 82.46, Z-Score: -2.45, Signal: BUY, Fundamental Driver: Risk Sentiment.

---

**👤 You:**
> "Check if the WTI and Brent oil pair is currently liquid enough to trade."

**🤖 AI Agent:**
> The liquidity check for WTI and Brent is complete. Both assets meet the minimum Open Interest requirement of 10,000.

---

**👤 You:**
> "What are the historical bounds for the gold/silver ratio?"

**🤖 AI Agent:**
> For the gold_silver pair, the 5-year minimum ratio spread is 55.0 and the maximum ratio spread is 95.0, driven by Risk Sentiment.


## ❓ FAQ

**Q: What kind of trading signals does this server provide?**
The server uses `analyze_spread_signals` to generate BUY or SELL signals based on z-score deviations from a 50-day moving average of the ratio spread, filtered by correlation and liquidity.

**Q: How does the engine ensure market liquidity?**
The engine uses `validate_liquidity_thresholds` to confirm that both assets in a pair have an Open Interest greater than 10,000 before a signal is considered valid.

**Q: Can I retrieve historical data for specific commodity pairs?**
Yes, you can use `get_historical_context` to retrieve the minimum and maximum ratio spreads and the fundamental economic drivers for specific pairs like gold/silver or WTI/Brent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/intermarket-spread-strategy](https://vinkius.com/ai-agent-connect/intermarket-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Intermarket Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `intermarket-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Intermarket Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intermarket-spread-strategy": {
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
