# Monthly Cashflow Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/monthly-cashflow-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate weekly liquidity projections and spending constraints based on income and bills.

## Description
This MCP server provides a financial planning engine to manage monthly liquidity. It connects AI agents to your financial schedule, allowing them to calculate weekly safe-to-spend amounts, identify potential shortfalls, and evaluate if savings goals are realistic. Use `calculate_weekly_budget` to see weekly discretionary limits, `check_liquidity_health` to detect if you will run out of money, `analyze_spending_capacity` to check if variable caps are achievable, and `get_monthly_summary` for a final month-end overview.


## Available Tools (4)
- **check_liquidity_health**: Identifies if the user will run out of money at any point during the month
- **calculate_weekly_budget**: Provides a week-by-week breakdown of how much money is available for discretionary spending
- **get_monthly_summary**: Provides a high-level overview of the month-end status
- **analyze_spending_capacity**: Determines if the user's variable spending caps and savings goals are realistic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monthly Cashflow Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have $2000 starting balance. I get $3000 on day 15. I have a $1200 rent bill on day 5 and a $500 savings goal for day 25. How much can I spend each week?"

**🤖 AI Agent:**
> Based on your schedule, your weekly safe-to-spend amounts are: Week 1: $400, Week 2: $300, Week 3: $600, Week 4: $400.

---

**👤 You:**
> "Will I run out of money this month if I have $500 starting balance, a $600 bill on day 10, and no other income?"

**🤖 AI Agent:**
> Yes, you will face a shortfall. Your balance will drop to -$100 on day 10.

---

**👤 You:**
> "Give me a summary of my month: $1000 start, $4000 total income, $2500 total bills, and $500 savings."

**🤖 AI Agent:**
> Your month-end status: Ending Balance: $2000, Total Inflow: $4000, Total Outflow: $3000, Net Cashflow: $1000.


## ❓ FAQ

**Q: How does the safe-to-spend calculation work?**
The `calculate_weekly_budget` tool determines available cash by subtracting upcoming fixed bills, necessary savings contributions, and a proportional portion of your variable spending caps from your current balance.

**Q: Can I detect if I will run out of money mid-month?**
Yes, use `check_liquidity_health` to identify if your balance will drop below zero at any point during the month and to see how many days of coverage you have.

**Q: How are savings goals handled?**
Savings goals are treated as planned outflows. The engine checks if your income and starting balance can cover both your fixed bills and your intended savings targets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/monthly-cashflow-planner](https://vinkius.com/en/ai-agent-connect/monthly-cashflow-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monthly Cashflow Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `monthly-cashflow-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monthly Cashflow Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "monthly-cashflow-planner": {
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
