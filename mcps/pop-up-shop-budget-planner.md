# Pop-up Shop Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pop-up-shop-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model operational costs and revenue targets for retail pop-up events.

## Description
This MCP server provides a specialized toolkit for retailers planning short-term pop-up events. It allows AI agents to calculate total operational expenditures, determine necessary sales targets to hit profit goals, and evaluate the profitability of projected revenue. Use `calculate_total_expenses` to aggregate booth, inventory, staff, travel, card fees, and decor costs. Use `calculate_sales_target` to find the revenue needed to cover costs plus a desired profit. Use `check_profitability` to verify if expected sales meet your minimum profit threshold, and `summary_budget_report` to identify your largest expense drivers.


## Available Tools (4)
- **calculate_sales_target**: Determine the exact amount of revenue needed to reach a specific profit goal
- **calculate_total_expenses**: Aggregate all individual cost categories into a single total budget figure
- **check_profitability**: Evaluate if a specific projected sales figure is sufficient to cover all costs and meet a profit threshold
- **summary_budget_report**: Provide a high-level breakdown of the budget distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pop-up Shop Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my total budget if my booth is $500, inventory is $1000, staff is $300, travel is $200, card fees are $50, and decor is $150?"

**🤖 AI Agent:**
> Your total budget is $2,200.

---

**👤 You:**
> "I have $2000 in total expenses. How much do I need to sell to make a $500 profit if my card fee is 3%?"

**🤖 AI Agent:**
> To achieve a $500 profit, your target sales must be $2,577.32.

---

**👤 You:**
> "Will I make at least $200 profit if I sell $3000 with $2000 in expenses and a 3% card fee?"

**🤖 AI Agent:**
> Yes, your actual profit will be $910.00, which exceeds your $200 threshold.


## ❓ FAQ

**Q: How do I calculate my total event costs?**
You can use the `calculate_total_expenses` tool by providing the costs for your booth, inventory, staff, travel, card fees, and decor.

**Q: Can this tool help me set a sales goal?**
Yes, the `calculate_sales_target` tool determines the exact revenue required to cover all expenses and achieve your specific desired profit margin.

**Q: How do I know if my pop-up will be profitable?**
Use the `check_profitability` tool. It compares your projected sales against your total expenses and minimum profit threshold to tell you if you will meet your goals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pop-up-shop-budget-planner](https://vinkius.com/en/ai-agent-connect/pop-up-shop-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pop-up Shop Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pop-up-shop-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pop-up Shop Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pop-up-shop-budget-planner": {
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
