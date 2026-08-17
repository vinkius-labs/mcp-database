# Reverse Cash-and-Carry Arbitrage Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reverse-cash-and-carry-arbitrage-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify and calculate deterministic arbitrage signals in backwardation markets.

## Description
This MCP server provides a deterministic engine to exploit backwardation by identifying underpriced futures. It calculates the theoretical fair value of contracts and generates precise trade signals. Use `calculate_arbitrage_signals` to detect entry points where the annualized basis is attractive, or `get_theoretical_fair_value` to compute the fair market value based on the cost of carry. The engine also includes `evaluate_risk_metrics` to assess market safety by analyzing borrowing costs and convenience yield volatility.


## Available Tools (3)
- **evaluate_risk_metrics**: Analyzes the risk profile of the current market environment to validate if the strategy is safe to execute
- **calculate_arbitrage_signals**: Determines if a trade signal is generated based on historical or daily market data and calculates position parameters
- **get_theoretical_fair_value**: Computes the fair market value of a futures contract at a specific point in time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reverse Cash-and-Carry Arbitrage Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate arbitrage signals for these prices: spot [100, 102], futures [95, 96], open interest [15000, 16000], days to expiry [45, 44], risk-free rate 0.03, borrowing cost 0.02, convenience yield 0.01, transaction costs 0.1."

**🤖 AI Agent:**
> The signal is a BUY futures and SELL spot position. Spot Price: 100, Futures Price: 95, Theoretical Price: 100.32, Basis: -5.0%, Annualized Yield: -8.2%, Days to Expiry: 45, Position Size: 1000, Margin Requirement: 5000.

---

**👤 You:**
> "What is the theoretical fair value for a spot price of 50 with a 4% risk-free rate, 2% convenience yield, and 30 days to expiry?"

**🤖 AI Agent:**
> The theoretical fair value is 50.08.

---

**👤 You:**
> "Evaluate the risk for a basis of -0.02, annualized basis of -0.09, borrowing cost of 0.04, and convenience yield volatility of 0.05."

**🤖 AI Agent:**
> The market is safe to trade. Risk Score: 0.45. Convenience Yield Risk Alert: False.


## ❓ FAQ

**Q: What is the primary market condition this tool targets?**
The engine specifically targets backwardation, where futures prices are lower than the spot price, allowing for a reverse cash-and-carry strategy.

**Q: How are trade signals generated?**
Signals are generated via `calculate_arbitrage_signals` when the actual futures price is lower than the theoretical fair value minus transaction costs, provided the annualized basis is below -8% and liquidity requirements are met.

**Q: Can I assess the risk of a trade before executing?**
Yes, you can use `evaluate_risk_metrics` to analyze the risk profile, including borrowing costs and potential spikes in convenience yield.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reverse-cash-and-carry-arbitrage-engine](https://vinkius.com/ai-agent-connect/reverse-cash-and-carry-arbitrage-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reverse Cash-and-Carry Arbitrage Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reverse-cash-and-carry-arbitrage-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reverse Cash-and-Carry Arbitrage Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reverse-cash-and-carry-arbitrage-engine": {
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
