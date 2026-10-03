# Student Budget Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/student-budget-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A monthly financial planning tool to balance income, academic costs, and living expenses.

## Description
Manage your student finances with precision. This MCP server provides tools to analyze budget health, calculate expense ratios, identify savings gaps, and suggest necessary spending cuts. Use `analyze_budget_health` to check if your income covers your costs, or `suggest_expense_cuts` to find ways to reach your savings goals.


## Available Tools (4)
- **analyze_budget_health**: Determines if a student's current financial plan is sustainable
- **find_savings_gap**: Identifies how much more income is needed to meet a specific savings target given current expenses
- **calculate_allocation_ratios**: Breaks down where the money is going as a percentage of the total budget
- **suggest_expense_cuts**: Suggests how much to reduce specific categories to reach a zero-deficit or target savings state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Student Budget Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my budget healthy? I have 2000 income, 800 rent, 400 food, 200 transport, 100 books, and I want to save 300."

**🤖 AI Agent:**
> Your budget is healthy. You have a surplus of 200.

---

**👤 You:**
> "How much more do I need to earn to save 500? My income is 1500, and my fixed expenses are 1200."

**🤖 AI Agent:**
> You need an additional 200 of income to meet your 500 savings goal.

---

**👤 You:**
> "I'm over budget. I have 1000 income, 700 rent, 300 food, 150 transport, 100 books, and I want to save 100. Where can I cut?"

**🤖 AI Agent:**
> To reach your goal, you need to reduce your non-rent expenses by 150. You could reduce food by 50, transport by 50, and books by 50.


## ❓ FAQ

**Q: How can I check if my budget is sustainable?**
You can use the `analyze_budget_health` tool by providing your total monthly income and your expected expenses like rent, food, and books.

**Q: What if I have a budget deficit?**
If you are overspending, use `suggest_expense_cuts` to receive specific recommendations on where to reduce spending in categories like food or transport.

**Q: Can I see the percentage breakdown of my spending?**
Yes, the `calculate_allocation_ratios` tool provides a detailed percentage breakdown of your rent, food, transport, books, and savings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/student-budget-builder](https://vinkius.com/en/ai-agent-connect/student-budget-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Student Budget Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `student-budget-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Student Budget Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "student-budget-builder": {
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
