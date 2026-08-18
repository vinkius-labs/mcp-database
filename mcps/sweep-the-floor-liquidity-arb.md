# Sweep the Floor Liquidity Arb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sweep-the-floor-liquidity-arb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Exploit thin liquidity in prediction markets by calculating price impact and exit strategies.

## Description
This MCP server provides deterministic tools to exploit thin liquidity in long-tail prediction markets. It allows AI agents to distinguish between mere illiquidity and genuine mispricing. Use `calculate_price_impact` to determine the cost of walking the order book, `evaluate_opportunity` to verify if the expected value (EV) exceeds the 0.10 threshold, and `generate_exit_strategy` to plan mean reversion trades by placing limit orders at the target mean price.


## Available Tools (3)
- **calculate_price_impact**: 
- **evaluate_opportunity**: 10

Evaluate if a trade is a viable arbitrage
- **generate_exit_strategy**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sweep the Floor Liquidity Arb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the price impact for buying $1000 worth of shares with a mid-price of 0.50 and this order book: [{"price": 0.51, "quantity": 500}, {"price": 0.55, "quantity": 1000}]"

**🤖 AI Agent:**
> The execution price is 0.52 and the total slippage is 4%.

---

**👤 You:**
> "Is a trade viable if I bought at 0.65 and the expected outcome price is 0.80?"

**🤖 AI Agent:**
> Yes, the expected value is 0.15, which is above the 0.10 threshold.

---

**👤 You:**
> "Generate an exit strategy for 500 shares entered at 0.50 with a target mean price of 0.55."

**🤖 AI Agent:**
> Place limit orders for 500 shares at 0.55 to capture a target spread of 0.05.


## ❓ FAQ

**Q: How does the tool handle slippage?**
The `calculate_price_impact` tool simulates walking the order book to calculate the volume-weighted average price (VWAP) and the resulting slippage.

**Q: What defines a viable trade?**
A trade is considered viable if `evaluate_opportunity` returns an expected value (EV) greater than 0.10 after accounting for execution costs.

**Q: Can I use this for exit planning?**
Yes, use `generate_exit_strategy` to calculate the optimal limit orders needed to capture the spread during mean reversion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sweep-the-floor-liquidity-arb](https://vinkius.com/ai-agent-connect/sweep-the-floor-liquidity-arb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sweep the Floor Liquidity Arb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sweep-the-floor-liquidity-arb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sweep the Floor Liquidity Arb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sweep-the-floor-liquidity-arb": {
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
