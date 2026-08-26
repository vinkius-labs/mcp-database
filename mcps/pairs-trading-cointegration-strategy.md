# Pairs Trading Cointegration Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pairs-trading-cointegration-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic pairs trading engine using Engle-Granger cointegration to identify mean-reverting asset pairs.

## Description
This MCP server provides a deterministic engine for pairs trading based on the Engle-Granger methodology. It allows AI agents to identify statistically significant cointegrated relationships between asset pairs and generate precise trading signals. Using `analyze_pair_cointegration`, agents can determine the hedge ratio, p-value, and half-life of mean reversion. Once a pair is validated, `generate_trading_signals` produces entry, exit, and stop-loss signals based on z-score deviations. Finally, `calculate_position_sizing` ensures trades remain dollar-neutral by calculating the exact quantities of each asset required based on the calculated hedge ratio.


## Available Tools (3)
- **analyze_pair_cointegration**: Determine if a specific pair of assets exhibits a statistically significant cointegrated relationship
- **generate_trading_signals**: Calculate daily z-scores and generate specific entry, exit, and stop-loss signals
- **calculate_position_sizing**: Determine the exact quantities of Asset A and Asset B to trade to maintain a dollar-neutral profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pairs Trading Cointegration Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the cointegration between these two price series: [100, 101, 102, 101, 100] and [50, 50.5, 51, 50.5, 50]."

**🤖 AI Agent:**
> The pair is cointegrated with a p-value of 0.03 and a hedge ratio of 0.5.

---

**👤 You:**
> "Generate trading signals for a pair with a hedge ratio of 1.5 and z-scores of 2.5, -0.1, and -2.5."

**🤖 AI Agent:**
> The first signal is BUY_SPREAD, the second is HOLD, and the third is SELL_SPREAD.

---

**👤 You:**
> "Calculate the position size for $10,000 capital with Asset A at $100, Asset B at $50, and a hedge ratio of 2.0."

**🤖 AI Agent:**
> To maintain a dollar-neutral position, you should trade 66.67 units of Asset A and 133.33 units of Asset B.


## ❓ FAQ

**Q: How does the engine confirm a pair is tradeable?**
The engine uses `analyze_pair_cointegration` to perform an ADF test. A pair is considered tradeable if the p-value is less than 0.05 and the half-life of mean reversion is below the specified limit.

**Q: What is a dollar-neutral position?**
A dollar-neutral position is achieved using `calculate_position_sizing`, where the total dollar value of the long position equals the total dollar value of the short position, minimizing market exposure.

**Q: Can I customize the entry and exit thresholds?**
Yes, the `generate_trading_signals` tool allows you to specify custom entry, exit, and stop-loss z-score thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pairs-trading-cointegration-strategy](https://vinkius.com/ai-agent-connect/pairs-trading-cointegration-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pairs Trading Cointegration Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pairs-trading-cointegration-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pairs Trading Cointegration Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pairs-trading-cointegration-strategy": {
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
