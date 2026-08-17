# Futures Ratio Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-ratio-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify 1:2 ratio spread entry signals using statistical Z-scores and market regime filters.

## Description
This MCP server provides deterministic quantitative tools for analyzing futures ratio spreads. It identifies high-probability entry signals for a 1:2 ratio spread (long 1 near-term, short 2 far-term) by monitoring spread Z-scores and market structure. Use `calculate_ratio_spread_signals` to evaluate historical price arrays and open interest for convergence opportunities. You can also use `get_market_regime_summary` to determine if the market is in contango or backwardation, and `validate_trade_feasibility` to ensure trades meet strict liquidity and margin requirements.


## Available Tools (3)
- **calculate_ratio_spread_signals**: Evaluates daily historical price data to identify specific entry signals for a 1:2 ratio spread
- **get_market_regime_summary**: Analyzes the current relationship between near and far contracts to determine market regime
- **validate_trade_feasibility**: Checks if a specific trade configuration meets the required safety and liquidity buffers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Ratio Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these historical prices for a 1:2 ratio spread: near prices [100, 101, 102, 101, 100], far prices [110, 112, 115, 113, 111], near OI [6000, 6100, 6200, 6150, 6050], far OI [7000, 7100, 7200, 7150, 7050], and risk capital 50000."

**🤖 AI Agent:**
> The analysis shows a LONG_SPREAD signal with a Z-score of 2.4, a spread value of 15, and a breakeven price of 115.

---

**👤 You:**
> "Is the market currently in contango if the near price is 105 and the far price is 102?"

**🤖 AI Agent:**
> No, the market is in backwardation because the near-term price is higher than the far-term price.

---

**👤 You:**
> "Check if a trade is feasible with a margin requirement of 1000, risk capital of 2000, near OI of 6000, and far OI of 6000."

**🤖 AI Agent:**
> The trade is not feasible because the risk capital is not at least three times the margin requirement.


## ❓ FAQ

**Q: What kind of ratio spread does this tool support?**
The tool is specifically designed for a 1:2 ratio spread, where you go long one near-term contract and short two far-term contracts.

**Q: How are entry signals generated?**
Signals are triggered when the spread Z-score exceeds 2.0 and the market is in a contango state, indicating a potential convergence opportunity.

**Q: Does the tool check for liquidity?**
Yes, the `validate_trade_feasibility` tool ensures that both contracts have an Open Interest greater than 5,000 before a trade is considered feasible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-ratio-spread-strategy](https://vinkius.com/ai-agent-connect/futures-ratio-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Ratio Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-ratio-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Ratio Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-ratio-spread-strategy": {
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
