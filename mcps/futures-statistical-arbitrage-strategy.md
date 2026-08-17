# Futures Statistical Arbitrage Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-statistical-arbitrage-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify mean-reverting opportunities between futures contracts using cointegration testing.

## Description
This MCP server provides deterministic statistical arbitrage tools for futures markets. It uses the Engle-Granger cointegration test to identify stable relationships between asset pairs. Users can use `analyze_pair_cointegration` to verify if a pair is mathematically suitable for trading based on liquidity and stationarity. Once a pair is validated, `generate_trading_signals` calculates precise entry, exit, and dollar-neutral position sizing based on z-score deviations. Additionally, `get_market_regime_summary` provides real-time health assessments of the asset relationship.


## Available Tools (3)
- **analyze_pair_cointegration**: Evaluates if two futures contracts are mathematically suitable for a mean-reversion strategy
- **generate_trading_signals**: Calculates entry, exit, and sizing instructions based on current spread deviation
- **get_market_regime_summary**: Provides a high-level summary of the relationship health between two assets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Statistical Arbitrage Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if Gold and Silver futures are suitable for a mean-reversion strategy using a 252-day lookback."

**🤖 AI Agent:**
> The pair is viable. The ADF p-value is 0.03, the half-life is 42 days, and both assets have sufficient liquidity.

---

**👤 You:**
> "Generate a trading signal for a spread with a z-score of 2.5, a hedge ratio of 1.2, and $100,000 available capital."

**🤖 AI Agent:**
> Signal: BUY_SPREAD. Position Size A: $50,000, Position Size B: $50,000 (adjusted by hedge ratio).

---

**👤 You:**
> "What is the current market regime for a pair with a p-value of 0.07 and a half-life of 30 days?"

**🤖 AI Agent:**
> The regime status is Weakly Cointegrated.


## ❓ FAQ

**Q: How does the system determine if a pair is tradeable?**
The system uses `analyze_pair_cointegration` to check if the pair has an ADF p-value below 0.10, a half-life of mean reversion under 60 days, and both assets have an Open Interest greater than 10,000.

**Q: What kind of signals are generated?**
The `generate_trading_signals` tool produces BUY_SPREAD, SELL_SPREAD, EXIT, or HOLD signals based on z-score thresholds, ensuring dollar-neutral position sizing.

**Q: Can I monitor the stability of the spread?**
Yes, you can use `get_market_regime_summary` to receive a status report such as 'Stable Cointegrated' or 'Unstable' based on the current p-value and half-life.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-statistical-arbitrage-strategy](https://vinkius.com/ai-agent-connect/futures-statistical-arbitrage-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Statistical Arbitrage Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-statistical-arbitrage-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Statistical Arbitrage Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-statistical-arbitrage-strategy": {
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
