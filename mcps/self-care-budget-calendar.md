# Self-Care Budget Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/self-care-budget-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan monthly self-care spending by synchronizing appointments and product replacement cycles.

## Description
Manage your wellness finances with precision. This MCP server connects your AI assistant to a specialized planning engine that synchronizes scheduled appointments and recurring product replacement cycles. Use `plan_monthly_budget` to calculate monthly costs within a specific savings cap, or `calculate_annual_projection` to forecast your total yearly wellness expenditure. It also provides tools like `get_product_replacement_schedule` to predict when skincare or supplements need repurchasing, and `check_budget_compliance` to ensure your planned spending stays within your financial limits.


## Available Tools (4)
- **check_budget_compliance**: Validates if a specific set of planned expenses violates the user's financial constraints
- **calculate_annual_projection**: Generates a full year-long spending forecast
- **get_product_replacement_schedule**: Determines which months a specific product will require a purchase
- **plan_monthly_budget**: Calculates the planned spending for a specific month given appointments and product cycles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Self-Care Budget Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan my budget for January with a $200 cap. I have a $150 massage and a $60 skincare product that needs replacing."

**🤖 AI Agent:**
> For January, your total allowed spend is $150. The massage is included, but the skincare product is deferred because the total would have exceeded your $200 cap.

---

**👤 You:**
> "What is my total projected spending for the year if my monthly budget is $100?"

**🤖 AI Agent:**
> Your total projected annual spending is $1,200.

---

**👤 You:**
> "Check if spending $250 is okay if my monthly limit is $200."

**🤖 AI Agent:**
> No, that spending is not compliant. You would exceed your limit by $50.


## ❓ FAQ

**Q: How does the budget prioritization work?**
If your planned spending exceeds your savings cap, the system uses `plan_monthly_budget` to prioritize items based on their importance, ensuring essential services are funded before luxury items.

**Q: Can I forecast my spending for the whole year?**
Yes, you can use the `calculate_annual_projection` tool to generate a full year-long spending forecast based on your monthly budget plans.

**Q: How do I know when to buy my skincare products again?**
You can use `get_product_replacement_schedule` to determine exactly which months a product will require a purchase based on its replacement interval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/self-care-budget-calendar](https://vinkius.com/en/ai-agent-connect/self-care-budget-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Self-Care Budget Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `self-care-budget-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Self-Care Budget Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "self-care-budget-calendar": {
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
