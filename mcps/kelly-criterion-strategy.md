# Kelly Criterion Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kelly-criterion-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic position sizing using the Kelly Criterion to manage trading capital.

## Description
This MCP server provides mathematical precision to trading capital management. It uses the Kelly Criterion to determine optimal position sizes based on your strategy's win rate and win/loss ratio. By applying a Half-Kelly safety buffer and enforcing a 25% concentration cap, it helps prevent over-exposure while maximizing long-term growth. Use `calculate_kelly_sizing` to find your optimal allocation, `evaluate_trade_parameters` to generate specific entry and exit instructions, and `analyze_strategy_expectancy` to evaluate your edge and risk of ruin.


## Available Tools (3)
- **analyze_strategy_expectancy**: 
- **calculate_kelly_sizing**: 
- **evaluate_trade_parameters**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kelly Criterion Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my position size for a strategy with a 55% win rate, a 2.0 win/loss ratio, and $50,000 in total capital."

**🤖 AI Agent:**
> Your optimal Half-Kelly position size is $5,500.

---

**👤 You:**
> "I have an entry price of $150, a stop-loss at $145, and a take-profit at $170. My allocated position size is $10,000. How many shares should I buy?"

**🤖 AI Agent:**
> You should purchase 66.67 shares.

---

**👤 You:**
> "What is the expected value and risk of ruin for a strategy with a 40% win rate, $500 average win, and $400 average loss?"

**🤖 AI Agent:**
> The expected value per trade is $20, and the estimated risk of ruin is 0.02%.


## ❓ FAQ

**Q: What is the Kelly Criterion?**
The Kelly Criterion is a formula used to determine the optimal size of a series of bets to maximize the logarithm of wealth, balancing win probability against the reward-to-risk ratio.

**Q: Why does the server use Half-Kelly sizing?**
Half-Kelly is a conservative approach that halves the theoretical Kelly percentage. This reduces volatility and provides a margin of safety against errors in estimating win rates or win/loss ratios.

**Q: How is the maximum position size limited?**
To prevent over-concentration, the server automatically caps any single position at 25% of your total available capital.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kelly-criterion-strategy](https://vinkius.com/ai-agent-connect/kelly-criterion-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kelly Criterion Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kelly-criterion-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kelly Criterion Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kelly-criterion-strategy": {
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
