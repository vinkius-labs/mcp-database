# Futures Options Calendar Spread Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-options-calendar-spread-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic decision engine for futures options calendar spreads using volatility term structure and time decay analysis.

## Description
This MCP server provides a deterministic decision engine for executing calendar spreads on futures options. By analyzing the relationship between near-term and far-term implied volatility (IV term structure), time decay (theta), and cost-to-strike ratios, it generates precise trading signals. Use `analyze_calendar_spread` to evaluate specific setups for BUY or SELL signals based on volatility backwardation or contango, liquidity filters, and gamma risk constraints. You can also use `calculate_spread_metrics` to derive specific components like the calendar spread debit and theta benefit.


## Available Tools (2)
- **analyze_calendar_spread**: Evaluates a specific calendar spread setup to generate a trading signal based on volatility, time, and cost constraints
- **calculate_spread_metrics**: Performs the underlying mathematical derivations for the spread components without generating a signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Options Calendar Spread Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this calendar spread: strike 4500, near-term premium 50, far-term premium 120, near-term 20 days to expiry, far-term 60 days to expiry, near-term IV 25%, far-term IV 20%, near-term OI 500, far-term OI 600."

**🤖 AI Agent:**
> Strike: 4500, Near-term Premium: 50, Far-term Premium: 120, Calendar Spread Debit: 70, IV Term Structure: -0.05, Max Profit: 150, Max Loss: 70, Signal Direction: BUY

---

**👤 You:**
> "Calculate the metrics for a spread with near-term premium 40, far-term premium 100, near-term IV 15%, far-term IV 22%, and strike 3800."

**🤖 AI Agent:**
> Calendar Spread Debit: 60, IV Term Structure: 0.07, Max Profit: 110, Max Loss: 60, Theta Benefit: 4.50

---

**👤 You:**
> "Should I trade a calendar spread with near-term 5 days to expiry and near-term IV 30% vs far-term IV 25%?"

**🤖 AI Agent:**
> No signal generated. The setup is skipped because near-term days to expiry is less than 7, which introduces excessive gamma risk.


## ❓ FAQ

**Q: What is a calendar spread?**
A calendar spread is an options strategy where a trader sells a near-term option and buys a far-term option at the same strike price.

**Q: How are trading signals generated?**
Signals are generated via `analyze_calendar_spread` by evaluating IV term structure, liquidity (Open Interest), and time to expiration to identify profitable volatility mispricings.

**Q: What are the liquidity requirements?**
The strategy requires both the near-term and far-term options to have an Open Interest (OI) greater than 300 to ensure sufficient market liquidity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-options-calendar-spread-strategy](https://vinkius.com/ai-agent-connect/futures-options-calendar-spread-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Options Calendar Spread Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-options-calendar-spread-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Options Calendar Spread Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-options-calendar-spread-strategy": {
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
