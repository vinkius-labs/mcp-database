# Family Grocery Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-grocery-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total and individual grocery expenditures for households.

## Description
This MCP server provides tools to manage household grocery budgets. You can use `get_total_cost` to find the total expenditure, `get_individual_share` to split a bill, `get_budget_variance` to check if you are over budget, and `get_household_summary` for a complete breakdown of metrics.

### Available Tools

`getTotalCostTool`, `getIndividualShareTool`, `getBudgetVarianceTool`, `getHouseholdSummaryTool`, `getTotalCost`, `getIndividualShare`, `getBudgetVariance`, `getHouseholdSummary`


## Available Tools (4)
- **getBudgetVariance**: Compare the actual grocery spending against a pre-planned budget
- **getHouseholdSummary**: Provide a complete breakdown of household grocery metrics
- **getIndividualShare**: Calculate how much a single person is responsible for when a total bill is known
- **getTotalCost**: Determine the total grocery expenditure for a family


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Grocery Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total grocery cost for a family of 4 where each person costs $50?"

**🤖 AI Agent:**
> The total grocery cost for a family of 4 at $50 per person is $200.

---

**👤 You:**
> "If the total grocery bill is $150 and there are 3 people, what is each person's share?"

**🤖 AI Agent:**
> Each person's share is $50.

---

**👤 You:**
> "I planned to spend $40 per person for 5 people, but the actual total was $220. Am I over budget?"

**🤖 AI Agent:**
> Yes, you are over budget by $20.


## ❓ FAQ

**Q: How do I calculate the total cost for my family?**
You can use the `get_total_cost` tool by providing the number of people in your household and the cost per person. Tools available: `getTotalCostTool`, `getIndividualShareTool`, `getBudgetVarianceTool`.

**Q: Can I check if I am over my grocery budget?**
Yes, the `get_budget_variance` tool compares your planned spending against the actual cost to show if you are over or under budget.

**Q: How is the individual share calculated?**
The `get_individual_share` tool divides the total grocery bill by the number of people in the household.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-grocery-cost-calculator](https://vinkius.com/en/ai-agent-connect/family-grocery-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Grocery Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-grocery-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Grocery Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-grocery-cost-calculator": {
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
