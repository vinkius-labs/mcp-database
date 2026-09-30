# Anniversary Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/anniversary-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare and optimize anniversary celebration scenarios.

## Description
This MCP server provides tools to plan and compare different anniversary celebration scenarios. You can use `compare_scenarios` to see side-by-side comparisons of cost and complexity, `calculate_scenario_total` to find the full price of a plan, `validate_budget_compliance` to ensure you stay within your spending limit, and `get_logistical_requirements` to identify necessary transport or childcare needs.


## Available Tools (4)
- **calculate_scenario_total**: Calculates the absolute financial and time cost of a single scenario
- **compare_scenarios**: Provides a side-by-side comparison of multiple anniversary plans
- **get_logistical_requirements**: Identifies physical resources needed for a scenario
- **validate_budget_compliance**: Checks if a scenario stays within a user-defined spending limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anniversary Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the 'Staycation' and 'European Trip' scenarios."

**🤖 AI Agent:**
> The 'Staycation' costs $500 with low complexity, while the 'European Trip' costs $4,500 with high complexity.

---

**👤 You:**
> "What is the total cost for scenario 'luxury_dinner_01'?"

**🤖 AI Agent:**
> The total cost for the luxury dinner scenario is $350.

---

**👤 You:**
> "Will scenario 'beach_getaway' fit in a $1,000 budget?"

**🤖 AI Agent:**
> Yes, the beach getaway costs $850, leaving you with $150 remaining in your budget.


## ❓ FAQ

**Q: How do I compare two different plans?**
Use the `compare_scenarios` tool by providing the unique IDs of the scenarios you want to evaluate side-by-side.

**Q: Can I check if a plan is too expensive?**
Yes, use `validate_budget_compliance` with your maximum budget to see if the scenario is within your limits.

**Q: How are logistical needs identified?**
The `get_logistical_requirements` tool analyzes the scenario to determine if you will need transport or childcare.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/anniversary-planner](https://vinkius.com/en/ai-agent-connect/anniversary-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Anniversary Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `anniversary-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Anniversary Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anniversary-planner": {
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
