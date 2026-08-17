# Liquid Staking Yield Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/liquid-staking-yield-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic optimization engine for LST trading signals.

## Description
This MCP server provides a deterministic optimization engine for generating daily trading signals for Liquid Staking Tokens (LSTs). By analyzing price deviations from underlying ETH, staking yields, and systemic risk filters, it identifies arbitrage opportunities. Use `analyze_lst_performance` to calculate historical discounts and real yields, `generate_trading_signals` to receive specific BUY or SELL instructions, and `summarize_strategy_exposure` to monitor portfolio positioning and risk metrics.


## Available Tools (3)
- **analyze_lst_performance**: Calculates historical discount, real yields, and comparative metrics for LSTs
- **generate_trading_signals**: Produces BUY, SELL, or HOLD instructions based on LST analysis and TVL
- **summarize_strategy_exposure**: Provides a high-level overview of current portfolio positioning and risk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liquid Staking Yield Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the performance of stETH given these prices and yields."

**🤖 AI Agent:**
> The analysis shows a discount of -2.5% and a real yield of 5.2%, which exceeds the lending rate.

---

**👤 You:**
> "Generate a trading signal for the current LST analysis."

**🤖 AI Agent:**
> BUY: The discount is -3% and staking APY is 4%, meeting all safety and yield criteria.

---

**👤 You:**
> "What is my current portfolio exposure?"

**🤖 AI Agent:**
> The current position is LONG with an average real yield of 4.8%.


## ❓ FAQ

**Q: What assets does this strategy support?**
The strategy is designed for Liquid Staking Tokens (LSTs) such as stETH and rETH by comparing them to the underlying ETH price.

**Q: How are trading signals generated?**
Signals are generated using `generate_trading_signals` based on discount thresholds, staking APY requirements, and TVL safety filters.

**Q: What is the purpose of the real yield calculation?**
The `analyze_lst_performance` tool calculates real yield by combining the staking APY with the expected profit from discount convergence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/liquid-staking-yield-strategy](https://vinkius.com/ai-agent-connect/liquid-staking-yield-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liquid Staking Yield Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `liquid-staking-yield-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liquid Staking Yield Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liquid-staking-yield-strategy": {
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
