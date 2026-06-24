# Portfolio Rebalancing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/portfolio-rebalancing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify portfolio drift and generate precise buy/sell orders to align asset weights with target allocations.

## Description
The Portfolio Rebalancing Engine connects AI agents to your investment strategy by identifying deviations from target asset allocations. Using the `analyze_portfolio_drift` tool, you can detect when assets have drifted beyond a specific threshold. The `compute_rebalancing_orders` tool generates the exact BUY and SELL instructions needed to restore your intended weights, while `estimate_rebalance_costs` calculates the transaction fees and net impact of these trades. This engine is ideal for maintaining risk profiles in automated trading or portfolio management workflows within Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools (3)
- **analyze_portfolio_drift**: Analyze portfolio drift
- **estimate_rebalancing_costs**: Estimate rebalancing costs
- **compute_rebalancing_orders**: Compute rebalancing orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Portfolio Rebalancing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My tech stock weight has drifted to 15% from a target of 10%. How much do I need to sell?"

**🤖 AI Agent:**
> To return your tech stock to the 10% target, you should execute a SELL order for the excess value relative to your total portfolio size.

---

**👤 You:**
> "Check if my current holdings are drifting from my target allocation."

**🤖 AI Agent:**
> The analysis shows that your 'Equities' asset is currently at 65% weight, while the target is 60%, indicating a drift of 5%.

---

**👤 You:**
> "What will be my total transaction cost if I execute these rebalancing orders with a 0.1% fee?"

**🤖 AI Agent:**
> Based on the provided orders, the estimated total transaction cost is $45.50, leaving you with a net portfolio value of $99,954.50.


## ❓ FAQ

**Q: How does the engine identify if rebalancing is needed?**
The `analyze_portfolio_drift` tool compares your current asset weights against your target allocations. If the difference (drift) exceeds your specified threshold, it flags the need for rebalancing.

**Q: What kind of orders does the tool generate?**
Using `compute_rebalancing_orders`, the engine generates specific BUY and SELL instructions, detailing the exact currency amount required for each asset to return to its target weight.

**Q: Can I estimate the cost of executing these trades?**
Yes, the `estimate_rebalancing_costs` tool allows you to input your trade orders and a fee rate to calculate total transaction costs and the resulting net portfolio value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portfolio-rebalancing-engine](https://vinkius.com/mcp/portfolio-rebalancing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Portfolio Rebalancing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `portfolio-rebalancing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Portfolio Rebalancing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "portfolio-rebalancing-engine": {
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
