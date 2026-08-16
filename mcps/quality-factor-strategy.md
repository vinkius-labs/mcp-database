# Quality Factor Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/quality-factor-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A quantitative tool to identify high-quality stocks using fundamental metrics.

## Description
This MCP server provides deterministic quantitative tools to capture the quality premium. It allows AI agents to compute composite quality scores using pillars like ROE, Debt-to-Equity, earnings stability, and dividend yield. Users can execute `calculate_quality_scores` to rank a universe of stocks, `generate_trading_signals` to determine long and short positions, and `analyze_strategy_performance` to evaluate risk metrics like quality beta and maximum drawdown.


## Available Tools (3)
- **analyze_strategy_performance**: Evaluates the historical effectiveness of the quality factor and its risk characteristics
- **calculate_quality_scores**: Computes the composite quality score for a set of stocks based on provided fundamental data
- **generate_trading_signals**: Determines the buy, sell, and hold actions for the portfolio based on quality rankings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quality Factor Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the quality scores for these stocks: [{'ticker': 'AAPL', 'roe': 0.25, 'debtToEquity': 1.5, 'earningsStability': 0.9, 'dividendYield': 0.01}, {'ticker': 'TSLA', 'roe': 0.15, 'debtToEquity': 0.5, 'earningsStability': 0.6, 'dividendYield': 0.0}] with equal weights."

**🤖 AI Agent:**
> {"scores": [{"ticker": "AAPL", "score": 0.75}, {"ticker": "TSLA", "score": 0.45}], "filteredStocks": ["AAPL", "TSLA"]}

---

**👤 You:**
> "Generate trading signals for these quality scores with a portfolio size of 1: [{'ticker': 'A', 'score': 0.9}, {'ticker': 'B', 'score': 0.5}, {'ticker': 'C', 'score': 0.1}]"

**🤖 AI Agent:**
> {"longList": [{"ticker": "A", "weight": 1.0}], "shortList": [{"ticker": "C", "weight": 1.0}], "holdList": ["B"], "canTrade": true}

---

**👤 You:**
> "Analyze the performance of the strategy using these returns and spread history: [{'returns': 0.05}, {'returns': -0.02}] and [{'spread': 0.03}, {'spread': 0.01}]"

**🤖 AI Agent:**
> {"qualitySpread": 0.02, "qualityBeta": 0.85, "maxDrawdown": 0.02, "benchmarkComparison": 0.015}


## ❓ FAQ

**Q: How are quality scores calculated?**
Scores are a weighted sum of ranks for ROE, inverse Debt-to-Equity, earnings stability, and dividend yield.

**Q: What are the filtering rules for stocks?**
The strategy excludes any stocks with negative earnings or an ROE below 5%.

**Q: Can I analyze the risk of my strategy?**
Yes, by using `analyze_strategy_performance`, you can calculate quality beta and maximum drawdown.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/quality-factor-strategy](https://vinkius.com/ai-agent-connect/quality-factor-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quality Factor Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quality-factor-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quality Factor Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quality-factor-strategy": {
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
