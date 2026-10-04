# Childcare Cost Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/childcare-cost-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Forecast childcare spending including fees, subsidies, and holiday closures.

## Description
This MCP server provides precise financial forecasting for childcare expenses. Use `calculate_weekly_cost` to determine base rates for multiple children, then use `forecast_annual_expenditure` to project yearly totals including registration fees and subsidies. You can also use `get_monthly_cash_flow` to see a month-by-month budget breakdown or `compare_childcare_options` to find the most cost-effective provider configuration.


## Available Tools (4)
- **compare_childcare_options**: Compares two different childcare configurations to find the most cost-effective option
- **forecast_annual_expenditure**: Generates a full-year financial forecast including all one-time fees and recurring costs
- **get_monthly_cash_flow**: Provides a granular view of monthly spending to assist with household budgeting
- **calculate_weekly_cost**: Determines the raw cost of childcare for a single week before subsidies or discounts are applied


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Childcare Cost Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the weekly cost for 2 children at $150 per hour for 40 hours?"

**🤖 AI Agent:**
> The total weekly cost for 2 children is $5,250.00, accounting for the multi-child discount on the second child.

---

**👤 You:**
> "Forecast my annual childcare cost for 1 child at $300/week with a $50 weekly subsidy and a $100 registration fee."

**🤖 AI Agent:**
> Your total annual cost is $12,500.00, which includes the $100 registration fee and accounts for the $50 weekly subsidy.

---

**👤 You:**
> "Show me the monthly budget breakdown for an annual cost of $10,000."

**🤖 AI Agent:**
> The monthly breakdown shows approximately $833.33 per month, with cumulative spending increasing each month from January through December.


## ❓ FAQ

**Q: How do I calculate the cost for multiple children?**
You can use the `calculate_weekly_cost` tool. It automatically applies multi-child discounts to the base rate for subsequent children.

**Q: Can I account for holidays when the center is closed?**
Yes, when using `forecast_annual_expenditure`, you can provide a list of week numbers where no care is provided to ensure those costs are excluded.

**Q: How are subsidies applied to my forecast?**
Subsidies can be applied as either a flat weekly amount or a percentage reduction using the `forecast_annual_expenditure` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/childcare-cost-planner](https://vinkius.com/en/ai-agent-connect/childcare-cost-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Childcare Cost Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `childcare-cost-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Childcare Cost Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "childcare-cost-planner": {
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
