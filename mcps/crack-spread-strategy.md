# Crack Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crack-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze refining margins and identify mean-reversion opportunities using a 3:2:1 crack spread model.

## Description
This MCP server provides a deterministic toolset for analyzing refining margins. By applying a 3:2:1 ratio model, it calculates the crack spread--the profit margin between crude oil and its refined products (gasoline and heating oil). The server uses statistical Z-Scores to identify mean-reversion opportunities: a low Z-Score indicates compressed margins (BUY signal), while a high Z-Score indicates expanded margins (SELL signal). It includes built-in liquidity filters and historical context analysis to ensure executable and informed trading decisions.


## Available Tools (3)
- **analyze_crack_spread**: Calculates the daily crack spread, statistical indicators, and generates trading signals
- **get_historical_context**: Retrieves the historical price range and seasonal trends
- **validate_market_liquidity**: Checks if the current market conditions meet the minimum requirements for profitable execution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crack Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current crack spread using recent crude, gasoline, and heating oil prices."

**🤖 AI Agent:**
> The current crack spread is $6.50 per barrel with a Z-Score of -2.2. Since the margin is above $5 and liquidity is sufficient, the signal is BUY (Short 3 Crude, Long 2 Gasoline, Long 1 Heating Oil).

---

**👤 You:**
> "Check if the market is liquid enough for a crack spread trade."

**🤖 AI Agent:**
> The market is liquid. All contracts meet the minimum open interest requirement of 10,000.

---

**👤 You:**
> "What are the historical seasonal trends for crack spreads?"

**🤖 AI Agent:**
> Historically, crack spreads tend to peak during the summer driving season due to increased gasoline demand.


## ❓ FAQ

**Q: What is the 3:2:1 ratio used in the analysis?**
The 3:2:1 ratio represents the standard refining yield where 3 barrels of crude oil produce 2 barrels of gasoline and 1 barrel of heating oil.

**Q: How are trading signals generated?**
Signals are generated using the `analyze_crack_spread` tool, which calculates a Z-Score. A BUY signal is triggered when the Z-Score is below -2.0, and a SELL signal when it is above 2.0, provided liquidity and margin requirements are met.

**Q: Does this tool check for market liquidity?**
Yes, the `validate_market_liquidity` tool ensures that all constituent contracts have an open interest greater than 10,000 before a signal is considered valid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crack-spread-strategy](https://vinkius.com/ai-agent-connect/crack-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crack Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crack-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crack Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crack-spread-strategy": {
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
