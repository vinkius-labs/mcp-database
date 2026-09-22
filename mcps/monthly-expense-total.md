# Monthly Expense Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/monthly-expense-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and aggregate monthly spending across categories.

## Description
This MCP server provides tools to manage and analyze monthly financial outflows. You can record new spending with `add_expense`, calculate the total sum for a specific period using `get_monthly_total`, view all items in a category via `list_expenses_by_category`, or see a full breakdown of spending with `get_category_distribution`.


## Available Tools (4)
- **add_expense**: Records a new expense into the system
- **get_category_distribution**: Provides a breakdown of spending across all categories for a specific month
- **get_monthly_total**: Calculates the total sum of all expenses for a specific month and year
- **list_expenses_by_category**: Retrieves a list of all expenses that fall under a specific category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Monthly Expense Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add an expense of 50 dollars for Groceries on 2024-05-15."

**🤖 AI Agent:**
> The expense of $50.00 for Groceries has been successfully recorded.

---

**👤 You:**
> "What was my total spending in March 2024?"

**🤖 AI Agent:**
> Your total spending for March 2024 was $1,250.00 across 12 expenses.

---

**👤 You:**
> "Show me all my expenses for the Rent category."

**🤖 AI Agent:**
> You have 3 expenses in the Rent category: $1200.00 on 2024-01-01, $1200.00 on 2024-02-01, and $1200.00 on 2024-03-01.


## ❓ FAQ

**Q: How do I add a new expense?**
You can use the `add_expense` tool by providing the amount, category, date, and an optional description.

**Q: Can I see how much I spent on food last month?**
Yes, you can use `list_expenses_by_category` for the 'Food' category or `get_category_distribution` to see the breakdown for that month.

**Q: How do I get my total spending for January 2024?**
Use the `get_monthly_total` tool with month 1 and year 2024.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/monthly-expense-total](https://vinkius.com/en/ai-agent-connect/monthly-expense-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Monthly Expense Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `monthly-expense-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Monthly Expense Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "monthly-expense-total": {
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
