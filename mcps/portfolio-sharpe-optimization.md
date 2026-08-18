# Portfolio Sharpe Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/portfolio-sharpe-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic capital allocation engine for maximizing Sharpe ratio in prediction markets.

## Description
This MCP server provides a deterministic capital allocation engine designed for prediction market participants. It uses Markowitz mean-variance optimization to calculate the exact weights needed to maximize the Sharpe ratio across multiple bets. Users can utilize `optimize_weights` to find optimal capital distribution, `get_efficient_frontier` to visualize risk-return trade-offs, and `analyze_risk_profile` to estimate maximum drawdown and receive automated rebalancing triggers when positions exceed 20% of the total portfolio.


## Available Tools (3)
- **analyze_risk_profile**: Estimates the potential downside and provides rebalancing instructions
- **get_efficient_frontier**: Generates a series of optimal portfolios to visualize the trade-off between risk and return
- **optimize_weights**: Calculates the exact capital allocation required to maximize the portfolio's Sharpe ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio Sharpe Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the optimal weights for these three markets: EVs of 0.15, 0.20, and 0.10; variances of 0.05, 0.06, and 0.04; a correlation matrix of [[1,0,0],[0,1,0],[0,0,1]]; and 1000 total capital."

**🤖 AI Agent:**
> The optimal allocation for your $1000 capital is: Market 1: $350.50, Market 2: $420.25, Market 3: $229.25. This configuration maximizes your Sharpe ratio based on the provided parameters.

---

**👤 You:**
> "What is my expected maximum drawdown if my current weights are {'market_a': 500, 'market_b': 500} with EVs of [0.1, 0.12], variances of [0.05, 0.05], and zero correlation?"

**🤖 AI Agent:**
> Based on your current holdings and market statistics, the estimated maximum drawdown is 8.4%.

---

**👤 You:**
> "Show me the efficient frontier for markets with EVs [0.2, 0.3], variances [0.04, 0.09], and a correlation of 0.2."

**🤖 AI Agent:**
> The efficient frontier has been calculated. The minimum variance portfolio offers an expected return of 0.22 with a volatility of 0.18, while the maximum return portfolio offers 0.30 with a volatility of 0.32.


## ❓ FAQ

**Q: How does the optimizer determine capital allocation?**
The engine uses Markowitz mean-variance optimization to solve for weights that maximize the Sharpe ratio, considering the expected values, variances, and correlations of all provided markets.

**Q: What triggers a rebalancing action?**
A rebalance action is automatically suggested via `analyze_risk_profile` if any single position grows to exceed 20% of the total portfolio value due to market price appreciation.

**Q: Can I visualize the risk-return trade-off?**
Yes, you can use the `get_efficient_frontier` tool to generate a series of optimal portfolios that map the relationship between volatility and expected return.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/portfolio-sharpe-optimization](https://vinkius.com/ai-agent-connect/portfolio-sharpe-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio Sharpe Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-sharpe-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio Sharpe Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-sharpe-optimization": {
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
