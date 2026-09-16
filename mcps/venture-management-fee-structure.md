# Venture Management Fee Structure MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-management-fee-structure)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate management fee economics, investable capital, and fee drag for VC funds.

## Description
This MCP server provides specialized financial modeling tools for venture capital fund management. It allows AI agents to perform complex economic calculations including total fee impact, investable capital availability, and the mathematical drag fees exert on investment returns. Key capabilities include using `calculate_fee_economics` to model fund-wide fee impacts, `analyze_step_down_impact` to evaluate fee reduction schedules, `calculate_investable_capital_with_recycling` to account for reinvested proceeds, and `estimate_fee_drag_on_returns` to quantify performance reduction.


## Available Tools (4)
- **calculate_investable_capital_with_recycling**: Determines the actual amount of capital available for deployment when exit proceeds are recycled
- **analyze_step_down_impact**: Evaluates how different fee reduction schedules affect the total lifetime fees
- **estimate_fee_drag_on_returns**: Quantifies the mathematical drag that management fees exert on the investment performance
- **calculate_fee_economics**: Calculates the total fee impact and capital availability for a fund


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Management Fee Structure** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fee economics for a $100M fund with a 2% fee and a 1.5% step-down in year 4."

**🤖 AI Agent:**
> The total fees for the $100M fund over its lifecycle, accounting for the step-down in year 4, are $18.5M, leaving $81.5M in investable capital.

---

**👤 You:**
> "What is the fee drag on a 3x MOIC if total fees are $5M on a $50M fund?"

**🤖 AI Agent:**
> The effective MOIC is 2.7x, resulting in a fee drag of 300 basis points.

---

**👤 You:**
> "How much capital is available if we recycle 20% of exits in a $50M fund with $5M in fees?"

**🤖 AI Agent:**
> The net investable capital is $45M, and the total deployed capital, including the 20% recycling, is $49M.


## ❓ FAQ

**Q: How does this tool help with fund modeling?**
It provides precise calculations for management fees, including the impact of step-down schedules and capital recycling on total investable capital.

**Q: Can I model fee reduction over time?**
Yes, you can use `analyze_step_down_impact` to compare different fee reduction schedules and see how they affect lifetime fees.

**Q: How is fee drag calculated?**
The `estimate_fee_drag_on_returns` tool calculates the effective MOIC and the drag in basis points by adjusting the target return by the ratio of fees to total capital.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-management-fee-structure](https://vinkius.com/en/ai-agent-connect/venture-management-fee-structure)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Management Fee Structure** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-management-fee-structure` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Management Fee Structure** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-management-fee-structure": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
