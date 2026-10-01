# Allowance Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/allowance-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Allocates child allowance into spending, saving, giving, and goal buckets.

## Description
This MCP server helps manage a child's allowance by dividing it into four distinct categories: Spending, Saving, Giving, and Goals. Using `get_allocation_summary`, you can see how the total allowance is distributed based on custom percentages. You can also use `get_weekly_balances` and `get_monthly_balances` to track remaining funds after accounting for recurring weekly and monthly purchases. Finally, `validate_allocation_rules` ensures that all percentage distributions and purchase lists are mathematically valid.


## Available Tools (4)
- **get_monthly_balances**: Calculates the total remaining funds in each bucket after a standard 4-week period, accounting for both weekly and monthly recurring costs
- **get_weekly_balances**: Determines the liquid amount left in each bucket at the end of a single week, accounting for weekly costs
- **validate_allocation_rules**: Validates if a set of percentages and purchase configurations are mathematically sound and follow the budget structure
- **get_allocation_summary**: Calculates how the total allowance is divided into the four primary buckets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Allowance Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If a child gets $50 a week and wants to split it 50% spending, 30% saving, 10% giving, and 10% goals, how much goes into each?"

**🤖 AI Agent:**
> The allocation is $25.00 for spending, $15.00 for saving, $5.00 for giving, and $5.00 for goals.

---

**👤 You:**
> "A child has a $40 allowance with 50% spending. They have a $5 weekly subscription in the spending category. What is the weekly balance for spending?"

**🤖 AI Agent:**
> The weekly spending balance is $15.00.

---

**👤 You:**
> "Calculate the monthly balance for a $100 allowance with 25% saving, where there is a $10 monthly purchase in the saving category."

**🤖 AI Agent:**
> The monthly saving balance is $90.00.


## ❓ FAQ

**Q: How does the allocation work?**
The total allowance is divided into four buckets based on the percentages you provide. You can use `get_allocation_summary` to see the exact dollar amounts for each category.

**Q: Can I account for recurring costs?**
Yes. You can use `get_weekly_balances` or `get_monthly_balances` to subtract recurring weekly or monthly purchases from the allocated amounts.

**Q: How do I know if my budget is valid?**
You can use the `validate_allocation_rules` tool to check if your percentages sum to 100% and if your purchase categories are correct.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/allowance-budget-planner](https://vinkius.com/en/ai-agent-connect/allowance-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Allowance Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `allowance-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Allowance Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "allowance-budget-planner": {
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
