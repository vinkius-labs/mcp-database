# Budget Category Percentage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/budget-category-percentage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate budget utilization and remaining percentages for specific categories.

## Description
This MCP server provides tools to manage and analyze budget allocations. You can use `get_category_utilization` to find the percentage of a total budget consumed by a single category, or `get_multiple_categories_status` to evaluate several categories at once. It also includes `validate_budget_integrity` to ensure category amounts do not exceed the total budget, and `get_budget_summary` to see the cumulative utilization across all categories.


## Available Tools (4)
- **validate_budget_integrity**: Checks if a specific category amount is valid within the context of a total budget
- **get_budget_summary**: Provides a high-level overview of total utilization across all provided categories
- **get_category_utilization**: Calculates what percentage of the total budget is consumed by a single category
- **get_multiple_categories_status**: Evaluates the status of several categories against a single total budget simultaneously


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Budget Category Percentage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What percentage of my $10,000 budget is used by a $2,500 marketing expense?"

**🤖 AI Agent:**
> The marketing expense uses 25% of your total budget, leaving 75% remaining.

---

**👤 You:**
> "Check if a $5,000 rent payment is valid for a $4,000 total budget."

**🤖 AI Agent:**
> No, the rent amount exceeds the total budget.

---

**👤 You:**
> "Give me a summary for a $5,000 budget with categories of $1,000, $500, and $1,500."

**🤖 AI Agent:**
> The total used percentage is 60%, and the total remaining percentage is 40%.


## ❓ FAQ

**Q: How do I check if a single category is within my budget?**
You can use the `validate_budget_integrity` tool to verify if a specific category amount is valid relative to your total budget.

**Q: Can I calculate the status of multiple categories at once?**
Yes, the `get_multiple_categories_status` tool allows you to evaluate a list of category amounts against a single total budget simultaneously.

**Q: How can I see the total percentage used by all my categories?**
Use the `get_budget_summary` tool to get a high-level overview of the cumulative used and remaining percentages for all provided categories.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/budget-category-percentage](https://vinkius.com/en/ai-agent-connect/budget-category-percentage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Budget Category Percentage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `budget-category-percentage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Budget Category Percentage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "budget-category-percentage": {
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
