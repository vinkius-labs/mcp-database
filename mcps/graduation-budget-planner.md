# Graduation Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/graduation-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and manage all costs for your graduation celebration.

## Description
This MCP server provides a complete financial toolkit for planning a graduation event. You can use `add_expense` to record costs for attire, photos, guests, travel, meals, gifts, and ceremony fees. Use `get_budget_summary` to see your remaining balance, `get_category_breakdown` to see where your money is going, and `calculate_guest_impact` to estimate the cost of inviting more people. It also includes `validate_budget_health` to ensure you stay within your spending limits.


## Available Tools (5)
- **calculate_guest_impact**: Estimates the cost implications of adding more guests to the celebration
- **get_budget_summary**: Provides a high-level overview of the current financial status
- **get_category_breakdown**: Analyzes how much money is being spent in each specific category
- **validate_budget_health**: Checks if the current spending is within safe limits
- **add_expense**: Records a new cost for a specific graduation category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Graduation Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just spent $150 on a new graduation gown. Can you add this to my budget?"

**🤖 AI Agent:**
> I have recorded the $150 expense for your graduation gown under the attire category. Your updated total spent is now updated.

---

**👤 You:**
> "How much have I spent on meals so far?"

**🤖 AI Agent:**
> You have spent a total of $240 on meals.

---

**👤 You:**
> "Is my budget still healthy if I want to keep a 10% safety margin?"

**🤖 AI Agent:**
> Yes, your budget is currently healthy and within your specified safety margin.


## ❓ FAQ

**Q: How do I add a new cost to my budget?**
You can use the `add_expense` tool to record any cost by specifying the category, the amount, and a brief description.

**Q: Can I see how much I have left to spend?**
Yes, use the `get_budget_summary` tool to view your total budgeted amount, total spent, and your remaining balance.

**Q: How does adding more guests affect my budget?**
You can use `calculate_guest_impact` to estimate the additional cost based on the number of new guests and the average cost per guest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/graduation-budget-planner](https://vinkius.com/en/ai-agent-connect/graduation-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Graduation Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `graduation-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Graduation Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "graduation-budget-planner": {
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
