# Budget Surplus Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/budget-surplus-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate net financial positions, income vs expense breakdowns, and category summaries.

## Description
This MCP server provides tools to manage and analyze budget data. Use `list_budget_periods` to find available timeframes, `get_net_position` to determine if a period has a surplus or deficit, `get_income_vs_expense_breakdown` for a high-level comparison, and `get_category_summary` to see how funds are distributed across categories.


## Available Tools (4)
- **get_net_position**: 
- **list_budget_periods**: 
- **get_category_summary**: 
- **get_income_vs_expense_breakdown**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Budget Surplus Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my net position for period P-2024-Q1?"

**🤖 AI Agent:**
> Your net position for period P-2024-Q1 is a SURPLUS of $1,250.00.

---

**👤 You:**
> "Show me the breakdown of income and expenses for period P-2024-Q1."

**🤖 AI Agent:**
> For period P-2024-Q1, your total income was $5,000.00 and your total expenses were $3,750.00, resulting in a difference of $1,250.00.

---

**👤 You:**
> "How much did I spend on groceries in period P-2024-Q1?"

**🤖 AI Agent:**
> In period P-2024-Q1, your total spending for the Groceries category was $450.00.


## ❓ FAQ

**Q: How do I see my current financial status?**
You can use the `get_net_position` tool to find out if you have a surplus or a deficit for a specific budget period.

**Q: Can I see a breakdown of my spending?**
Yes, use `get_category_summary` to see how much is attributed to specific categories like rent or groceries.

**Q: What budget periods are available?**
You can call `list_budget_periods` to retrieve all recorded timeframes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/budget-surplus-calculator](https://vinkius.com/en/ai-agent-connect/budget-surplus-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Budget Surplus Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `budget-surplus-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Budget Surplus Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "budget-surplus-calculator": {
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
