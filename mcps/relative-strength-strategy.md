# Relative Strength Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/relative-strength-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A deterministic momentum strategy identifying assets outperforming a benchmark.

## Description
This MCP server provides tools to execute a deterministic momentum strategy. It identifies high-momentum assets by comparing their performance against a benchmark like SPY. Using `calculate_rs_metrics`, you can derive RS values, slope, and percentile rank. The `evaluate_strategy_signals` tool determines BUY, SELL, or HOLD actions based on RS moving average crossovers and trend filters. Finally, `perform_monthly_rebalance` allows for periodic portfolio rotation into the top 3 assets by RS strength.


## Available Tools (3)
- **calculate_rs_metrics**: Calculates core relative strength indicators and momentum characteristics
- **evaluate_strategy_signals**: Determines trade actions (BUY, SELL, HOLD) and risk parameters
- **perform_monthly_rebalance**: Identifies top assets for the next monthly period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative Strength Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the relative strength metrics for these asset prices and benchmark prices."

**🤖 AI Agent:**
> The current RS value is 1.25 with a positive slope and a percentile rank of 85%.

---

**👤 You:**
> "Should I buy this asset based on the current signals?"

**🤖 AI Agent:**
> BUY signal triggered: RS is above the moving average, slope is positive, and the asset is in an uptrend.

---

**👤 You:**
> "What are the top 3 assets to hold for the next month?"

**🤖 AI Agent:**
> The top 3 assets for the next period are AAPL, MSFT, and NVDA.


## ❓ FAQ

**Q: What is the core logic of the strategy?**
The strategy triggers a BUY when the RS is above its moving average, the RS slope is positive, and both the asset and the benchmark are in an uptrend.

**Q: How are stop-losses handled?**
A stop-loss is triggered if the price falls below the 200-day moving average or drops 10% below the entry price.

**Q: How often does the portfolio rebalance?**
The strategy performs a monthly rebalance, rotating the portfolio into the top 3 assets based on their RS percentile rank.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/relative-strength-strategy](https://vinkius.com/ai-agent-connect/relative-strength-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative Strength Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-strength-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative Strength Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-strength-strategy": {
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
