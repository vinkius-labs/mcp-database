# Renovation Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/renovation-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Track renovation costs, phase summaries, and cash flow timelines.

## Description
This MCP server provides tools to manage renovation finances. Use `get_phase_summaries` to monitor the status of individual stages, `get_project_financial_health` to check the total budget and contingency, `get_cash_flow_timeline` to schedule upcoming payments, and `get_overbudget_items` to identify specific cost overruns.


## Available Tools (4)
- **get_cash_flow_timeline**: Provides a chronological schedule of required payments to ensure liquidity
- **get_overbudget_items**: Identifies specific line items (labor, materials, or permits) that have exceeded their estimated value
- **get_phase_summaries**: Provides a high-level overview of the financial status of each renovation phase
- **get_project_financial_health**: Answers how much money has been "locked in" versus the total planned budget including contingency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Renovation Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of the financial status for each phase in project PROJ-123."

**🤖 AI Agent:**
> The Demolition phase has an estimated cost of $5,000 and a committed cost of $5,200, meaning it is over budget. The Plumbing phase has an estimated cost of $12,000 and a committed cost of $10,000.

---

**👤 You:**
> "What is the total planned budget and remaining contingency for project PROJ-123?"

**🤖 AI Agent:**
> The total planned budget is $50,000 and the remaining contingency is $2,500.

---

**👤 You:**
> "Show me the payment schedule for project PROJ-123 starting from 2024-05-01."

**🤖 AI Agent:**
> On 2024-05-15, you have a $1,200 payment for plumbing materials. On 2024-06-01, there is a $3,000 payment for electrical labor.


## ❓ FAQ

**Q: How can I see if a specific phase is over budget?**
You can use the `get_phase_summaries` tool to see the estimated versus committed costs for every phase in your project.

**Q: How do I plan for upcoming expenses?**
Use the `get_cash_flow_timeline` tool to generate a chronological schedule of all required payments.

**Q: What is the total amount of money I have committed so far?**
You can find the total committed amount by calling `get_project_financial_health` for your specific project ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/renovation-budget-planner](https://vinkius.com/en/ai-agent-connect/renovation-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Renovation Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renovation-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Renovation Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renovation-budget-planner": {
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
