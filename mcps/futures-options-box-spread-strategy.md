# Futures Options Box Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-options-box-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Detect deterministic arbitrage opportunities in futures options box spreads.

## Description
This MCP server provides a deterministic engine to identify mispriced box spreads in futures options. By comparing the market cost of a four-legged position against its theoretical present value, it identifies arbitrage opportunities. Use `analyze_box_spread` to calculate profitability and signal direction, `calculate_margin_and_risk` to estimate capital requirements, and `get_market_liquidity_status` to ensure sufficient market depth for execution.


## Available Tools (3)
- **calculate_margin_and_risk**: Estimates the capital required to hold the position and the inherent danger of the execution
- **get_market_liquidity_status**: Validates if the specific options contracts are liquid enough to support arbitrage
- **analyze_box_spread**: Calculates the cost, theoretical value, and profitability of a specific box spread configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Options Box Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a box spread with K1=100, K2=110, call K1 premium=5, call K2 premium=2, put K1 premium=3, put K2 premium=6, futures price=105, risk-free rate=0.05, days to expiry=30, and all legs having OI of 1000 and spread of 0.5%."

**🤖 AI Agent:**
> The box spread cost is 0.00 and the theoretical value is 9.92. Since the cost is less than 99% of the theoretical value, the signal is BUY.

---

**👤 You:**
> "Check the liquidity for four option contracts with the following data: [{'oi': 600, 'spread': 0.01}, {'oi': 800, 'spread': 0.01}, {'oi': 550, 'spread': 0.01}, {'oi': 1200, 'spread': 0.01}]."

**🤖 AI Agent:**
> The market is liquid. All contracts meet the minimum Open Interest threshold of 500.

---

**👤 You:**
> "Calculate the margin and execution risk for a box spread with a cost of 10.0 and a strike difference of 10.0, where the liquidity score is 1000."

**🤖 AI Agent:**
> The estimated margin requirement is 1.0 and the execution risk is Low.


## ❓ FAQ

**Q: What is a box spread arbitrage?**
A box spread is a neutral strategy using two calls and two puts at different strikes. Arbitrage occurs when the cost to enter this position is significantly different from the discounted value of the guaranteed payoff at expiration.

**Q: How does the engine handle liquidity?**
The engine uses `get_market_liquidity_status` to verify that all four option legs have sufficient Open Interest and narrow bid-ask spreads before confirming a trade signal.

**Q: What are the execution risks?**
The primary risk is legging risk, where one part of the trade is filled but others are not. You can use `calculate_margin_and_risk` to assess these risks based on market depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-options-box-spread-strategy](https://vinkius.com/ai-agent-connect/futures-options-box-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Options Box Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-options-box-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Options Box Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-options-box-spread-strategy": {
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
