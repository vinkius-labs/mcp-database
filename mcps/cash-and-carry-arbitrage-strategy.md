# Cash-and-Carry Arbitrage Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cash-and-carry-arbitrage-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify and track deterministic futures arbitrage opportunities by exploiting contango.

## Description
This MCP server provides quantitative tools to identify and manage cash-and-carry arbitrage opportunities. By analyzing the discrepancy between spot and futures prices, users can detect contango markets where the futures price exceeds the theoretical fair value. The server includes `analyze_arbitrage_signals` to detect entry and exit points based on liquidity and annualized basis, `calculate_position_economics` to determine locked-in profit and capital efficiency, and `monitor_basis_risk` to evaluate the stability of the arbitrage spread.


## Available Tools (3)
- **monitor_basis_risk**: Evaluates the stability of the arbitrage opportunity by tracking the volatility of the basis
- **analyze_arbitrage_signals**: Identifies daily arbitrage entry and exit signals based on price discrepancies and liquidity constraints
- **calculate_position_economics**: Computes the expected financial outcomes of a specific arbitrage trade once a signal is identified


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cash-and-Carry Arbitrage Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze current market data for arbitrage opportunities."

**🤖 AI Agent:**
> The current annualized basis is 14.5% with an open interest of 15,000 contracts, signaling a valid entry opportunity.

---

**👤 You:**
> "Calculate the expected profit for an entry at $100 spot and $105 futures."

**🤖 AI Agent:**
> The locked-in profit is $3.50 with a capital efficiency of 12.5% after accounting for all financing and transaction costs.

---

**👤 You:**
> "Check the risk level for my current basis history."

**🤖 AI Agent:**
> The current basis volatility is low, resulting in a Low risk assessment for this arbitrage position.


## ❓ FAQ

**Q: What is a cash-and-carry arbitrage?**
It is a strategy where an investor buys a physical asset (spot) and simultaneously sells a futures contract to lock in a risk-free profit when the market is in contango.

**Q: How does the tool determine an entry signal?**
Using `analyze_arbitrage_signals`, an entry is triggered if the actual futures price is higher than the theoretical price plus costs, the annualized basis exceeds 10%, and open interest is above 10,000 contracts.

**Q: Can I assess the risk of my position?**
Yes, you can use `monitor_basis_risk` to evaluate the volatility of the basis and determine the qualitative risk level of your arbitrage position.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cash-and-carry-arbitrage-strategy](https://vinkius.com/ai-agent-connect/cash-and-carry-arbitrage-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cash-and-Carry Arbitrage Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cash-and-carry-arbitrage-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cash-and-Carry Arbitrage Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cash-and-carry-arbitrage-strategy": {
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
