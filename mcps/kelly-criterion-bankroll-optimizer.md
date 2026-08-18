# Kelly Criterion Bankroll Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kelly-criterion-bankroll-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic position sizing for binary prediction markets using Kelly Criterion math.

## Description
This MCP server provides a suite of mathematical tools for managing bankrolls in binary prediction markets. It uses the Kelly Criterion to calculate optimal bet sizes based on the edge between market prices and your estimated true probabilities. Users can use `calculate_kelly_position` to find specific bet amounts, `simulate_strategy_performance` to forecast long-term growth and risk of ruin, or `validate_market_edge` to quickly assess if a market opportunity is profitable. All calculations include safety multipliers and a strict 5% position cap to protect capital.


## Available Tools (3)
- **calculate_kelly_position**: Calculates the recommended bet size for a single market opportunity
- **validate_market_edge**: Quickly determines if a market opportunity is worth pursuing
- **simulate_strategy_performance**: Estimates the long-term behavior and risks of a specific betting strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kelly Criterion Bankroll Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a $1000 bankroll. The market price for a 'Yes' outcome is 0.4, but I think the true probability is 0.5. What should my bet size be using Half-Kelly?"

**🤖 AI Agent:**
> With a $1000 bankroll, a market price of 0.4, and a true probability of 0.5, your recommended bet size using Half-Kelly is $12.50.

---

**👤 You:**
> "Is there an edge in a market where the price is 0.7 and my estimated probability is 0.6?"

**🤖 AI Agent:**
> No, there is no profitable edge in this market because the true probability is lower than the market price.

---

**👤 You:**
> "Simulate 100 bets with a $500 bankroll, market price 0.5, true probability 0.55, and a 0.25 safety multiplier."

**🤖 AI Agent:**
> The simulation for 100 bets shows an expected growth rate of 0.002 per bet, a risk of ruin of 0.0%, and a maximum drawdown of 1.2%.


## ❓ FAQ

**Q: How does the position sizing cap work?**
The server enforces a hard 5% cap on any single bet. Even if `calculate_kelly_position` suggests a larger amount, the recommended bet size will never exceed 5% of your current bankroll.

**Q: What is the difference between Full Kelly and Half-Kelly?**
Full Kelly uses the raw mathematical fraction. Half-Kelly uses a `safetyMultiplier` of 0.5, which reduces the bet size to half of the full Kelly amount to decrease volatility and drawdown risk.

**Q: Can I simulate long-term outcomes?**
Yes, you can use `simulate_strategy_performance` to run a simulation of consecutive bets to estimate your expected growth rate and the probability of a 90% drawdown.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kelly-criterion-bankroll-optimizer](https://vinkius.com/ai-agent-connect/kelly-criterion-bankroll-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kelly Criterion Bankroll Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kelly-criterion-bankroll-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kelly Criterion Bankroll Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kelly-criterion-bankroll-optimizer": {
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
