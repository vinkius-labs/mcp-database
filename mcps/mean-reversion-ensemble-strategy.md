# Mean-Reversion Ensemble Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mean-reversion-ensemble-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

An algorithmic trading engine that uses an ensemble of RSI, Bollinger Bands, and Z-Score to identify high-probability mean-reversion entries.

## Description
This MCP server provides a deterministic ensemble strategy for identifying mean-reversion opportunities. By aggregating three distinct technical indicators--RSI, Bollinger Bands, and Z-Score--the engine confirms extreme market conditions through an ensemble scoring mechanism. Users can use `calculate_ensemble_signals` to generate technical indicators, `generate_trading_plan` to derive specific entry and exit parameters, and `analyze_reversion_probability` to evaluate the historical success rate of specific ensemble scores. This approach ensures that trades are only initiated when multiple signals align, reducing the risk of false signals in volatile markets.


## Available Tools (3)
- **analyze_reversion_probability**: 
- **calculate_ensemble_signals**: 
- **generate_trading_plan**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mean-Reversion Ensemble Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate technical signals for these closing prices: [150.2, 148.5, 145.0, 142.1, 140.5, 141.2, 143.5]"

**🤖 AI Agent:**
> The signal series has been generated. The final bar shows an oversoldScore of 3, indicating a potential BUY signal.

---

**👤 You:**
> "Create a trading plan for the following signal series: [{"timestamp": 1625097600, "rsi": 25, "bbLower": 145, "bbUpper": 160, "zScore": -2.5, "oversoldScore": 3, "overboughtScore": 0, "signalType": "BUY"}]"

**🤖 AI Agent:**
> The trading plan is ready. Entry Price: 140.5, Stop-Loss: 136.38, Take-Profit: 150.2.

---

**👤 You:**
> "What is the historical probability of reversion for an ensemble score of 3?"

**🤖 AI Agent:**
> Based on the provided signal series, an ensemble score of 3 has a historical reversion probability of 68.5%.


## ❓ FAQ

**Q: What is an ensemble score in this strategy?**
The ensemble score is a count (0 to 3) of how many indicators (RSI, Bollinger Bands, and Z-Score) simultaneously signal an extreme oversold or overbought condition.

**Q: When does the strategy trigger a BUY signal?**
A BUY signal is triggered only when the `oversoldScore` reaches exactly 3, meaning RSI, Bollinger Bands, and Z-Score all confirm an oversold state.

**Q: How is the stop-loss calculated?**
The stop-loss is determined by the higher of a 3% drop from the entry price or the price level where the ensemble score drops to 1.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mean-reversion-ensemble-strategy](https://vinkius.com/ai-agent-connect/mean-reversion-ensemble-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mean-Reversion Ensemble Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mean-reversion-ensemble-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mean-Reversion Ensemble Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mean-reversion-ensemble-strategy": {
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
