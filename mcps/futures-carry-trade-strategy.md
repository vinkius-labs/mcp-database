# Futures Carry Trade Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-carry-trade-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify arbitrage opportunities by comparing implied market carry against theoretical cost-of-carry models.

## Description
This MCP server provides a deterministic engine for executing futures carry trade strategies. It identifies arbitrage opportunities by calculating the difference between implied market carry and the theoretical cost-of-carry (risk-free rate + storage costs - convenience yield). Use `get_daily_signals` to generate BUY or SELL signals based on market regimes like Contango or Backwardation. You can also use `calculate_carry_performance` to analyze historical P&L and roll-down returns, or `analyze_market_regime` to classify the current state of the futures curve.


## Available Tools (3)
- **analyze_market_regime**: Classifies the current state of the futures curve
- **get_daily_signals**: Provides the primary trading signals by comparing implied market carry against theoretical model carry
- **calculate_carry_performance**: Analyzes the historical profitability of the carry strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Carry Trade Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for these front-month prices [100, 101, 102], second-month prices [105, 106, 107], risk-free rate 0.05, storage cost 0.01, convenience yield 0.02, front OI [15000, 16000, 17000], second OI [12000, 13000, 14000], and 30 days between months."

**🤖 AI Agent:**
> The signal for the latest date is BUY, with an implied carry of 16.1% and a theoretical carry of 4.0%.

---

**👤 You:**
> "What is the current market regime if the front-month price is 50 and the second-month price is 48 with 30 days between months?"

**🤖 AI Agent:**
> The market is in Backwardation.

---

**👤 You:**
> "Calculate the performance for a signal history of [{'date': '2023-01-01', 'signalDirection': 'BUY'}] and front-month prices [100, 105]."

**🤖 AI Agent:**
> The cumulative carry P&L is 5.0 and the roll-down return is 2.5.


## ❓ FAQ

**Q: How are trading signals generated?**
Signals are generated via `get_daily_signals` by comparing the implied carry from the futures curve against the theoretical cost-of-carry model, filtered by liquidity and volatility constraints.

**Q: What is the difference between Contango and Backwardation?**
Contango occurs when the second-month price is higher than the front-month price, while Backwardation occurs when the second-month price is lower than the front-month price.

**Q: How can I evaluate the strategy's historical success?**
You can use the `calculate_carry_performance` tool to compute cumulative P&L and roll-down returns based on historical signal and price data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-carry-trade-strategy](https://vinkius.com/ai-agent-connect/futures-carry-trade-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Carry Trade Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-carry-trade-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Carry Trade Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-carry-trade-strategy": {
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
