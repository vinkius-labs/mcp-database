# Annual Expense Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/annual-expense-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate projected annual expenditures based on monthly spending.

## Description
This MCP server provides tools to manage and project budget data. Use `get_monthly_expenses` to retrieve specific spending, `calculate_annual_projection` to extrapolate monthly costs to a full year, `get_category_summary` for category breakdowns, and `get_yearly_budget_report` for a complete overview of all projected annual costs.


## Available Tools (4)
- **calculate_annual_projection**: Answers how much a user will spend in a year based on a single month's spending
- **get_category_summary**: Provides an overview of all monthly expenses recorded under a specific category
- **get_monthly_expenses**: Retrieves the recorded expense amount for a specific category within a specific month
- **get_yearly_budget_report**: Generates a full report of projected annual costs across all expense categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Annual Expense Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will I spend in a year if my monthly food expense is $500?"

**🤖 AI Agent:**
> Your projected annual expenditure for food is $6,000.

---

**👤 You:**
> "Give me a summary of my housing expenses."

**🤖 AI Agent:**
> In the Housing category, you spent $1,200 in January and $1,200 in February, with an average monthly spend of $1,200.

---

**👤 You:**
> "What is my total projected annual budget for all categories?"

**🤖 AI Agent:**
> Your total projected annual expenditure across all categories is $45,000.


## ❓ FAQ

**Q: How do I calculate my yearly spending for a specific category?**
You can use `get_category_summary` to see the monthly breakdown and average spend for that category.

**Q: Can I project my total annual budget?**
Yes, use `get_yearly_budget_report` to generate a full report of projected annual costs across all categories.

**Q: How do I find out what I spent in January?**
Use the `get_monthly_expenses` tool by providing the category name and 'January' as the month.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/annual-expense-total](https://vinkius.com/en/ai-agent-connect/annual-expense-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Annual Expense Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `annual-expense-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Annual Expense Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "annual-expense-total": {
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
