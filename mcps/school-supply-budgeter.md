# School Supply Budgeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-supply-budgeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and manage school supply costs with ease.

## Description
This MCP server provides essential tools for parents and educators to manage school supply budgets. Use `list_available_supplies` to browse the catalog, `calculate_item_subtotal` for individual item costs, `aggregate_shopping_list` to find the grand total including tax, and `validate_budget_limit` to ensure your spending stays within your planned budget.


## Available Tools (4)
- **aggregate_shopping_list**: Calculates the total cost, tax, and grand total for a list of items
- **list_available_supplies**: Lists available school supplies from the catalog
- **calculate_item_subtotal**: Calculates the subtotal for a specific quantity of an item
- **validate_budget_limit**: Checks if a shopping list fits within a budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Supply Budgeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What school supplies are available in the writing category?"

**🤖 AI Agent:**
> The writing category includes Pencils, Pens, Highlighters, and Erasers.

---

**👤 You:**
> "How much will 5 Pencils cost?"

**🤖 AI Agent:**
> 5 Pencils will cost $2.50.

---

**👤 You:**
> "Calculate the total for 2 Notebooks and 10 Pencils with a 7% tax rate."

**🤖 AI Agent:**
> The total budget is $5.00, the tax amount is $0.35, and the grand total is $5.35.


## ❓ FAQ

**Q: How do I see what supplies are available?**
You can use the `list_available_supplies` tool to view the full catalog of items and their unit prices.

**Q: Can I calculate the total cost including tax?**
Yes, the `aggregate_shopping_list` tool allows you to provide a tax rate to calculate the grand total.

**Q: How can I check if I am over my budget?**
Use the `validate_budget_limit` tool to check if your list of items fits within your specified budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-supply-budgeter](https://vinkius.com/en/ai-agent-connect/school-supply-budgeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Supply Budgeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-supply-budgeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Supply Budgeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-supply-budgeter": {
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
