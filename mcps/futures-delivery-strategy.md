# Futures Delivery Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/futures-delivery-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify arbitrage and liquidity squeezes in futures markets.

## Description
This MCP server provides deterministic algorithmic tools to monitor the convergence between futures and spot markets. Use `analyze_market_state` to detect liquidity squeezes when supply is tight and basis is high. Determine trade directions with `get_trading_signal` based on arbitrage logic, and use `calculate_delivery_economics` to compute total costs and squeeze probabilities for physical delivery strategies.


## Available Tools (3)
- **get_trading_signal**: Determines the specific trade direction (BUY, SELL, or HOLD) based on arbitrage and squeeze logic
- **analyze_market_state**: Provides a daily snapshot of the relationship between futures and spot prices and the current supply conditions
- **calculate_delivery_economics**: Computes the total costs and probability factors associated with executing a physical delivery strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Futures Delivery Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current market state with a basis of 6% and 5,000 contracts available."

**🤖 AI Agent:**
> A squeeze is detected due to high basis and tight supply.

---

**👤 You:**
> "What is the trading signal if the basis is -6% and supply is 60,000?"

**🤖 AI Agent:**
> The signal is BUY.

---

**👤 You:**
> "Calculate the delivery economics for a spot price of 100 with 5 storage and 2 insurance costs."

**🤖 AI Agent:**
> The total delivery cost is 7.


## ❓ FAQ

**Q: How do I detect a delivery squeeze?**
A squeeze is detected using `analyze_market_state` when the days to first notice is under 30, the basis is above 5%, and deliverable supply is below 10,000 contracts.

**Q: What determines a BUY signal?**
A BUY signal is generated via `get_trading_signal` when the basis is less than -5% and the deliverable supply is greater than 50,000.

**Q: Can I calculate delivery costs?**
Yes, use `calculate_delivery_economics` to compute total delivery costs including storage, insurance, and transportation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/futures-delivery-strategy](https://vinkius.com/ai-agent-connect/futures-delivery-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Futures Delivery Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `futures-delivery-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Futures Delivery Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "futures-delivery-strategy": {
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
