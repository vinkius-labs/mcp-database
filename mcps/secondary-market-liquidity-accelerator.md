# Secondary Market Liquidity Accelerator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/secondary-market-liquidity-accelerator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimates cash value and optimal exit timing for private equity stakes.

## Description
This MCP server provides specialized modeling to estimate the cash value and timing of exiting private equity stakes within accelerator-backed portfolios. It calculates potential liquidity, discount impacts, and optimal exit windows by analyzing market demand and transfer restrictions. Use `get_potential_liquidity` to estimate realized cash value, `get_optimal_exit_timing` to find the best year to sell, and `evaluate_market_constraints` to assess how buyer availability and legal hurdles affect feasibility.


## Available Tools (3)
- **evaluate_market_constraints**: Determines how restrictions and buyer availability impact the feasibility of a sale
- **get_potential_liquidity**: Calculates the estimated cash value a holder can expect to receive from a secondary sale
- **get_optimal_exit_timing**: Identifies the most advantageous year to sell the stake to maximize realized value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Secondary Market Liquidity Accelerator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the potential liquidity for a 10% stake in an asset with a 15% discount and strong market demand after 3 years?"

**🤖 AI Agent:**
> The estimated potential cash value for your 10% stake is $850,000, with a discount impact of $150,000.

---

**👤 You:**
> "When is the best time to exit my position given current market conditions?"

**🤖 AI Agent:**
> The optimal exit year is Year 5, where you are projected to achieve a maximum realized value of $2,400,000.

---

**👤 You:**
> "How will a small buyer universe affect my sale?"

**🤖 AI Agent:**
> A small buyer universe will increase the required liquidity premium and may result in an estimated delay of 1.5 years to complete the transaction.


## ❓ FAQ

**Q: How do I estimate the cash I will receive from a sale?**
You can use the `get_potential_liquidity` tool. Provide the portfolio equity percentage, market demand, discount rate, and how long you have held the asset to get an estimate of the potential cash value.

**Q: Can this tool help me decide when to sell my stake?**
Yes, the `get_optimal_exit_timing` tool identifies the most advantageous year to sell by projecting asset growth against market discount rates.

**Q: How are transfer restrictions accounted for?**
The `evaluate_market_constraints` tool specifically analyzes how the size of the buyer universe and the level of transfer restrictions impact the feasibility and timing of a sale.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/secondary-market-liquidity-accelerator](https://vinkius.com/ai-agent-connect/secondary-market-liquidity-accelerator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Secondary Market Liquidity Accelerator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `secondary-market-liquidity-accelerator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Secondary Market Liquidity Accelerator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "secondary-market-liquidity-accelerator": {
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
