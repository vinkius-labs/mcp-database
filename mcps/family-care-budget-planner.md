# Family Care Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-care-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate caregiving expenses, contributor schedules, and reimbursement tracking.

## Description
This MCP server provides a comprehensive financial orchestration layer for managing caregiving costs. It connects AI agents to your family's care budget, allowing for precise management of recurring costs and one-time expenses. Use `get_monthly_spending_plan` to view budget allocations, `get_contributor_schedule` to manage payment timelines, `get_shortfall_actions` to address funding gaps, and `get_reimbursement_checklist` to track payments owed to contributors. It is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Available Tools (4)
- **get_contributor_schedule**: Generates a calendar of when each person needs to pay their committed amount
- **get_monthly_spending_plan**: Provides a detailed view of how much money is allocated to specific costs for a given month
- **get_reimbursement_checklist**: Provides a tracking list for money that needs to be paid back to contributors
- **get_shortfall_actions**: Identifies how to handle the gap when expenses exceed available funds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Care Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the spending plan for March 2024."

**🤖 AI Agent:**
> In March 2024, the total monthly burn is $2,500. The medical supplies category is allocated $1,200, and the caregiver wages are allocated $1,300.

---

**👤 You:**
> "When does John need to make his contribution in May 2024?"

**🤖 AI Agent:**
> John is scheduled to contribute $500 on 2024-05-15.

---

**👤 You:**
> "Are there any shortfalls for June 2024?"

**🤖 AI Agent:**
> Yes, there is a shortfall of $300 for June 2024. It is recommended to reduce non-priority expenses to cover this gap.


## ❓ FAQ

**Q: How can I see my monthly budget allocation?**
You can use the `get_monthly_spending_plan` tool to see a detailed breakdown of category allocations and the total monthly burn.

**Q: What happens if my expenses exceed my budget?**
The `get_shortfall_actions` tool will identify the deficit and provide recommended steps to address the gap, such as reducing non-priority expenses.

**Q: How do I track money owed to family members?**
Use the `get_reimbursement_checklist` tool to view a list of pending and completed reimbursements for expenses paid by contributors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-care-budget-planner](https://vinkius.com/en/ai-agent-connect/family-care-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Care Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-care-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Care Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-care-budget-planner": {
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
