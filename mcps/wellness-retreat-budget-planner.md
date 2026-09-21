# Wellness Retreat Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellness-retreat-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Precision financial modeling for wellness retreats, calculating total costs, per-person pricing, and break-even occupancy.

## Description
This MCP server provides a complete financial engine for planning wellness retreats. It allows planners to model complex cost structures including lodging, treatments, meals, and transport. Use `calculate_total_budget` to generate a full breakdown with taxes and contingencies, or `analyze_profitability` to find the minimum number of guests needed to break even. You can also use `get_daily_spend_forecast` to visualize daily cash flow or `compare_budget_scenarios` to evaluate how changing guest counts affects your margins.


## Available Tools (4)
- **analyze_profitability**: Determines the financial feasibility of a retreat
- **calculate_total_budget**: Calculates the complete financial breakdown of a retreat
- **compare_budget_scenarios**: Compares two different budget configurations
- **get_daily_spend_forecast**: Provides a granular view of daily spending


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellness Retreat Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total budget for a 5-night retreat for 15 guests with $200 lodging per night, $150 treatments, $50 class fees, $40 meals per day, $500 fixed transport, 8% tax, 10% service fee, and 15% contingency."

**🤖 AI Agent:**
> The total budget for the retreat is $23,456.50, with a per-person cost of $1,563.77.

---

**👤 You:**
> "If my total budget is $15,000 and I charge $1,200 per person, how many guests do I need to break even?"

**🤖 AI Agent:**
> You need at least 13 guests to reach the break-even point.

---

**👤 You:**
> "Show me the daily spending forecast for a 3-night retreat with 10 guests, $200 daily fixed costs, and $150 daily variable costs per person."

**🤖 AI Agent:**
> The daily spend for each of the 3 days is $1,700.00, with an average daily spend of $1,700.00.


## ❓ FAQ

**Q: How do I calculate the minimum number of guests needed?**
You can use the `analyze_profitability` tool. Provide the total budget, the price you intend to charge per person, and the expected guest count to find your break-even occupancy.

**Q: Can I see a day-by-day breakdown of expenses?**
Yes, the `get_daily_spend_forecast` tool provides a granular view of daily spending, including fixed and variable costs for each day of the retreat.

**Q: Does the budget include taxes and service fees?**
Yes, when using `calculate_total_budget`, you can specify tax and service fee rates to ensure the final total includes all mandatory levies and fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellness-retreat-budget-planner](https://vinkius.com/en/ai-agent-connect/wellness-retreat-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellness Retreat Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellness-retreat-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellness Retreat Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellness-retreat-budget-planner": {
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
