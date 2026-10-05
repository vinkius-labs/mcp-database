# Freelance Utilization Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/freelance-utilization-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Predict freelance revenue and capacity by modeling billable hours, rates, and overhead.

## Description
This MCP server provides a suite of tools for freelancers to model their future earnings. Use `get_capacity_forecast` to determine available billable hours, `calculate_revenue_projections` to estimate gross income, and `calculate_net_earnings` to find take-home pay after overhead. You can also use `get_utilization_summary` to analyze your efficiency and profit margins.


## Available Tools (4)
- **calculate_net_earnings**: Determines the actual take-home pay after accounting for business expenses
- **calculate_revenue_projections**: Predicts total gross revenue based on billable capacity and rates
- **get_capacity_forecast**: Calculates the total available billable hours for a freelancer over a specific period
- **get_utilization_summary**: Provides a high-level overview of efficiency and profitability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freelance Utilization Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many billable hours will I have over the next 4 weeks if I have a holiday on July 4th?"

**🤖 AI Agent:**
> Based on a standard capacity, you will have 152 billable hours available over the next 4 weeks after accounting for the holiday.

---

**👤 You:**
> "What will my gross revenue be if I work 120 billable hours at $75 per hour?"

**🤖 AI Agent:**
> Your total gross revenue will be $9,000.

---

**👤 You:**
> "If I earn $5,000 and my overhead is $1,200, what is my net earnings?"

**🤖 AI Agent:**
> Your net earnings will be $3,800.


## ❓ FAQ

**Q: How do I calculate my expected monthly income?**
You can use `calculate_revenue_projections` by providing your expected billable hours and your hourly rate.

**Q: Can I account for holidays in my capacity planning?**
Yes, the `get_capacity_forecast` tool allows you to pass a list of holiday dates to adjust your total available hours.

**Q: How is my profit margin calculated?**
The `get_utilization_summary` tool calculates your profit margin as the ratio of net earnings to gross revenue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/freelance-utilization-forecast](https://vinkius.com/en/ai-agent-connect/freelance-utilization-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freelance Utilization Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freelance-utilization-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freelance Utilization Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freelance-utilization-forecast": {
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
