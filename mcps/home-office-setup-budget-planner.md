# Home Office Setup Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-office-setup-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan and optimize your workspace budget based on physical constraints, ergonomics, and financial limits.

## Description
This MCP server provides a suite of tools to help you design the perfect workspace. You can use `get_workspace_fit` to ensure your furniture fits your room, `validate_ergonomics` to check health compliance, `calculate_total_expenditure` to manage costs including tax and shipping, and `generate_budget_report` to see your final financial status. It bridges the gap between physical space planning and financial management.


## Available Tools (4)
- **calculate_total_expenditure**: Calculates the final cost of the setup including all taxes and shipping
- **get_workspace_fit**: Determines if a set of selected furniture can physically fit within the specified workspace dimensions
- **generate_budget_report**: Compiles a complete overview of the setup plan
- **validate_ergonomics**: Checks if the selected equipment configuration meets the user's health and comfort requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Office Setup Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Will a 120x60x75cm desk fit in a room that is 200x200x250cm?"

**🤖 AI Agent:**
> Yes, the desk fits within the workspace dimensions with significant remaining volume.

---

**👤 You:**
> "Calculate the total cost for a chair costing $150 with 10% tax and $20 shipping."

**🤖 AI Agent:**
> $185.00

---

**👤 You:**
> "Generate a budget report for a $500 budget with a $450 total cost and a missing chair."

**🤖 AI Agent:**
> The remaining budget is $50.00, and the required item 'chair' is still unfulfilled.


## ❓ FAQ

**Q: How do I know if my desk will fit in my room?**
You can use the `get_workspace_fit` tool by providing your room's dimensions and the dimensions of the furniture you intend to buy.

**Q: Does the budget include taxes and shipping?**
Yes, the `calculate_total_expenditure` tool accounts for both tax rates and shipping fees to give you a precise final cost.

**Q: Can I check if my setup is healthy for my posture?**
Yes, the `validate_ergonomics` tool checks your equipment against specific ergonomic constraints like desk height and monitor eye level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-office-setup-budget-planner](https://vinkius.com/en/ai-agent-connect/home-office-setup-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Office Setup Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-office-setup-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Office Setup Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-office-setup-budget-planner": {
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
