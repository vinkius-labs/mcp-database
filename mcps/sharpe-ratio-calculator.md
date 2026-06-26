# Sharpe Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sharpe-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate advanced risk-adjusted performance metrics like Sharpe, Sortino, and Calmar ratios.

## Description
This MCP server provides precise financial tools to evaluate investment quality using risk-adjusted performance metrics. Use `get_market_benchmark` to retrieve annualized risk-free rates for the USA, Europe, or Brazil markets. The `calculate_asset_metrics` tool allows you to analyze a single series of returns to determine Sharpe, Sortino, and Calmar ratios along with a performance tier (Poor, Good, or Excellent). For multi-asset analysis, use `calculate_portfolio_metrics` to compute weighted aggregate metrics for an entire portfolio based on provided asset weights.


## Available Tools (3)
- **calculate_asset_metrics**: g., [0.01, -0.02, 0.05]) and the market context to calculate risk-improved performance metrics.

Calculates Sharpe, Sortino, and Calmar ratios for a single series of periodic returns
- **calculate_portfolio_metrics**: Calculates aggregated performance metrics for a collection of assets with specific weightings
- **get_market_benchmark**: g., Fed Funds, ECB, or Selic) for USA, Europe, or Brazil markets.

Retrieves the current risk-free rate for a selected geographic market


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sharpe Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the risk-free rate for the USA market?"

**🤖 AI Agent:**
> The annualized risk-free rate for the USA market is 5.33%.

---

**👤 You:**
> "Calculate metrics for these monthly returns in Brazil: [0.02, -0.01, 0.03, 0.01, -0.02]"

**🤖 AI Agent:**
> For the provided returns in Brazil, the Sharpe Ratio is 1.45, the Sortino Ratio is 1.82, and the Calmar Ratio is 2.10, resulting in a Good performance tier.

---

**👤 You:**
> "Analyze a portfolio with two assets: Asset A (returns [0.05, 0.02], weight 0.6) and Asset B (returns [0.01, -0.01], weight 0.4) in the Europe market."

**🤖 AI Agent:**
> The aggregate portfolio metrics for the Europe market are: Sharpe Ratio: 1.25, Sortino Ratio: 1.40, and Calmar Ratio: 1.85.


## ❓ FAQ

**Q: What markets are supported for risk-free rate retrieval?**
The `get_market_benchmark` tool currently supports the USA (Federal Funds Rate), Europe (ECB rate), and Brazil (Selic rate).

**Q: How is investment performance classified?**
Performance is categorized into three tiers: Poor (ratio < 1.0), Good (1.0 to 2.0), and Excellent (ratio > 2.0).

**Q: Can I calculate metrics for a group of assets at once?**
Yes, use the `calculate_portfolio_metrics` tool by providing a JSON string containing the returns series and weights for each asset in your portfolio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sharpe-ratio-calculator](https://vinkius.com/mcp/sharpe-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sharpe Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sharpe-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sharpe Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sharpe-ratio-calculator": {
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
