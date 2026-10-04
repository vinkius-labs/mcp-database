# Portfolio Rebalance Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/portfolio-rebalance-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A precision engine for calculating automated trade instructions to align holdings with target allocations.

## Description
This MCP server provides a precision engine for managing investment portfolios. It calculates exact buy and sell orders required to align current holdings with desired target allocations while optimizing for available cash. Users can use `calculate_rebalance_plan` to generate specific trade lists, `get_current_allocation` to analyze existing drift, `validate_portfolio_health` to assess risk, and `simulate_what_if_allocation` to project the impact of changing target weights.


## Available Tools (4)
- **calculate_rebalance_plan**: Generates a detailed plan of buy and sell orders to reach target allocations
- **get_current_allocation**: Calculates the current distribution of assets compared to target allocations
- **simulate_what_if_allocation**: Simulates the theoretical outcome of changing target allocations
- **validate_portfolio_health**: Evaluates if the current portfolio drift is within healthy limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio Rebalance Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a rebalance plan for my holdings: [{assetId: 'BTC', quantity: 0.5}, {assetId: 'USD', quantity: 1000}] with prices: [{assetId: 'BTC', price: 50000}, {assetId: 'USD', price: 1}] and targets: [{assetId: 'BTC', targetPercentage: 80}, {assetId: 'USD', targetPercentage: 20}]."

**🤖 AI Agent:**
> To reach your target allocation, you should sell 0.02 BTC and buy 0.01 BTC (simulated result). Your residual cash will be $100 and your final allocation will be 80% BTC and 20% USD.

---

**👤 You:**
> "Is my portfolio healthy? Holdings: [{assetId: 'AAPL', quantity: 10}] Prices: [{assetId: 'AAPL', price: 150}] Targets: [{assetId: 'AAPL', targetPercentage: 100}]."

**🤖 AI Agent:**
> Your portfolio is healthy with a total drift of 0% and no misaligned assets.

---

**👤 You:**
> "What is my current allocation? Holdings: [{assetId: 'ETH', quantity: 10}] Prices: [{assetId: 'ETH', price: 2000}] Targets: [{assetId: 'ETH', targetPercentage: 100}] Cash: 500."

**🤖 AI Agent:**
> Your current ETH allocation is 97.5% with a target of 100%, resulting in a drift of 2.5%.


## ❓ FAQ

**Q: How does the rebalancing plan handle available cash?**
The engine prioritizes selling assets to generate liquidity first, then uses available cash to fulfill buy orders. If cash is insufficient, buy orders are scaled to respect liquidity constraints.

**Q: Can I simulate changes before executing trades?**
Yes, you can use the `simulate_what_if_allocation` tool to project the theoretical outcome of new target percentages without executing actual trades.

**Q: What defines a 'healthy' portfolio in this tool?**
A portfolio is considered healthy if the maximum drift for any single asset remains below the system's defined sensitivity threshold, as determined by `validate_portfolio_health`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/portfolio-rebalance-planner](https://vinkius.com/en/ai-agent-connect/portfolio-rebalance-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio Rebalance Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-rebalance-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio Rebalance Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-rebalance-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
