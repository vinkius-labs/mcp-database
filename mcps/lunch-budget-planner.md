# Lunch Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lunch-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize your workday lunch spending and maximize monthly savings.

## Description
The Lunch Budget Planner helps you balance the cost of home-prepared meals against restaurant alternatives. By using tools like `calculate_daily_plan` and `get_monthly_summary`, you can generate weekly schedules, check if your lunch plan is sustainable with `validate_budget_feasibility`, and compare the financial impact of eating out versus preparing meals with `compare_meal_types`.


## Available Tools (4)
- **compare_meal_types**: Analyzes the cost-benefit ratio between home preparation and eating out
- **calculate_daily_plan**: Generates a weekly schedule of meals and calculates the total savings achieved by preparing meals
- **get_monthly_summary**: Provides a high-level financial overview of the lunch strategy for the month
- **validate_budget_feasibility**: Checks if a specific lunch configuration is sustainable within a given monthly budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lunch Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a $300 monthly budget. A prepared meal costs $5 and a restaurant meal costs $15. I want to prepare meals 3 days a week. What is my plan?"

**🤖 AI Agent:**
> Your weekly schedule will include 3 prepared meals and 2 restaurant meals. Your total monthly cost will be $150, resulting in $150 in savings.

---

**👤 You:**
> "Is it feasible to spend $10 on home meals and $20 on restaurants 4 days a week with a $250 monthly budget?"

**🤖 AI Agent:**
> No, that plan is not feasible. The projected monthly cost is $360, which exceeds your $250 budget by $110.

---

**👤 You:**
> "Compare the cost of a $6 home meal versus a $18 restaurant meal."

**🤖 AI Agent:**
> Choosing a prepared meal saves you $12 per meal, which is a 66.67% savings. You can buy 3 prepared meals for the price of 1 restaurant meal.


## ❓ FAQ

**Q: How does the planner calculate savings?**
Savings are calculated by comparing the cost of eating at a restaurant every workday against the cost of your hybrid plan using `calculate_daily_plan`.

**Q: Can I check if my budget is enough for my meal plan?**
Yes, you can use the `validate_budget_feasibility` tool to see if your proposed lunch configuration fits within your monthly limit.

**Q: What is a 'Prepared' meal?**
A prepared meal is a lunch you make at home or pre-prepare, which typically costs less than buying food from a restaurant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lunch-budget-planner](https://vinkius.com/en/ai-agent-connect/lunch-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lunch Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lunch-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lunch Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lunch-budget-planner": {
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
