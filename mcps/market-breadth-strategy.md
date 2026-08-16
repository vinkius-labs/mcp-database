# Market Breadth Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/market-breadth-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic quantitative trading signals using market breadth indicators.

## Description
This MCP server provides deterministic quantitative trading signals by analyzing market breadth. It uses the `analyze_breadth_signals` tool to generate BUY, SELL, and HOLD signals based on the interaction between price trends and internal strength. It also includes `calculate_breadth_metrics` for momentum indicators like the McClellan Oscillator and breadth divergence, and `get_breadth_summary` for a high-level snapshot of market health.


## Available Tools (3)
- **analyze_breadth_signals**: Generates the primary trading signals (BUY, SELL, HOLD) based on the interaction between price trends and internal breadth strength
- **calculate_breadth_metrics**: Computes secondary momentum and divergence indicators to support the primary signal logic
- **get_breadth_summary**: Provides a high-level snapshot of current market health based on the most recent data point


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Market Breadth Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current market status and score?"

**🤖 AI Agent:**
> The current market status is Expanding with a breadth score of 3.

---

**👤 You:**
> "Generate a trading signal based on these index prices and ADL values."

**🤖 AI Agent:**
> The signal is BUY with an entry price of 4500.00, a stop-loss at 4275.00, and a take-profit at 4950.00.

---

**👤 You:**
> "Are there any momentum indicators like divergence or thrust?"

**🤖 AI Agent:**
> The current metrics show a McClellan Oscillator of 5.2 and no active breadth divergence.


## ❓ FAQ

**Q: What determines a BUY signal?**
A BUY signal is generated when the Breadth Score is 3, the index price is above its 50-day moving average, and the McClellan Oscillator is positive.

**Q: How is the Breadth Score calculated?**
The score is the sum of three binary checks: positive ADL slope, new highs exceeding new lows, and over 50% of stocks above their 20-day MA.

**Q: What is a Breadth Thrust?**
A Breadth Thrust is an aggressive bullish signal where the Advance/Decline Line increases by more than 10% over a 10-day period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/market-breadth-strategy](https://vinkius.com/ai-agent-connect/market-breadth-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Market Breadth Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `market-breadth-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Market Breadth Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "market-breadth-strategy": {
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
