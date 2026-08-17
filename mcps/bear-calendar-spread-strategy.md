# Bear Calendar Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bear-calendar-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generates deterministic trading signals for bear calendar spreads using spread z-scores and contango analysis.

## Description
This MCP server provides a deterministic engine for executing bear calendar spread strategies. It monitors the relationship between near-term and far-term futures contracts to identify profitable opportunities. By analyzing spread volatility through z-scores and ensuring market contango, the engine identifies when spreads have expanded too far or are reverting to the mean. Users can use `calculate_spread_signals` to generate daily trade directions, `get_spread_economics` to calculate cost of carry and convergence targets, and `validate_contract_suitability` to ensure liquidity requirements are met before execution.


## Available Tools (3)
- **calculate_spread_signals**: Generates daily trading signals based on spread volatility, contango status, and z-scores
- **get_spread_economics**: Provides detailed financial metrics regarding the cost and targets of the current spread state
- **validate_contract_suitability**: Verifies if two specific contracts are eligible for the strategy based on underlying asset and liquidity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bear Calendar Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate trading signals for these near-term prices [100, 101, 102] and far-term prices [105, 106, 107] with near-term OI [6000, 6100, 6200] and far-term OI [7000, 7100, 7200]."

**🤖 AI Agent:**
> The signals generated for the provided price arrays are: Day 1: HOLD, Day 2: HOLD, Day 3: SELL.

---

**👤 You:**
> "Calculate the economics for a spread where the near-term price is 100 and the far-term price is 105."

**🤖 AI Agent:**
> The spread width is 5, the cost of carry is 5, and the convergence target is the historical mean.

---

**👤 You:**
> "Check if these contracts are suitable: near-term underlying is GOLD, far-term underlying is GOLD, near-term OI is 10000, far-term OI is 12000."

**🤖 AI Agent:**
> The contracts are eligible for the strategy.


## ❓ FAQ

**Q: What is a bear calendar spread?**
A bear calendar spread involves selling a near-term futures contract and buying a far-term contract to profit from the narrowing of the spread.

**Q: How does the engine determine a SELL signal?**
A SELL signal is triggered when the spread z-score exceeds 2.0 and the market is in contango, indicating the spread has expanded significantly.

**Q: What liquidity requirements are enforced?**
The strategy requires both the near-term and far-term contracts to have an Open Interest (OI) greater than 5,000 to ensure sufficient liquidity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bear-calendar-spread-strategy](https://vinkius.com/ai-agent-connect/bear-calendar-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bear Calendar Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bear-calendar-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bear Calendar Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bear-calendar-spread-strategy": {
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
