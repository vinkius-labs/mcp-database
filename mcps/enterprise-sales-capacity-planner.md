# Enterprise Sales Capacity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-sales-capacity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate sales headcount, revenue capacity, and hiring timelines.

## Description
This MCP server provides a complete capacity planning engine for sales organizations. It calculates total revenue capacity by accounting for AE tenure and ramp schedules, identifies the capacity gap against growth targets, and forecasts necessary hiring needs including turnover replacements. Use `generate_hiring_timeline` to create monthly hiring schedules that ensure new hires reach full productivity exactly when needed.


## Available Tools (4)
- **calculate_capacity_gap**: Identifies the shortfall between current team performance and future revenue goals
- **forecast_hiring_needs**: Determines how many new AEs must be hired to close the capacity gap
- **generate_hiring_timeline**: Creates a monthly schedule of when hiring must occur to meet capacity targets
- **get_current_capacity**: Determines the total revenue capacity of the existing sales team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Sales Capacity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current sales capacity if we have two AEs with $500k quota at 10 months tenure and one AE at 2 months tenure with $500k quota?"

**🤖 AI Agent:**
> Your current total capacity is $1,100,000, assuming the new hire is at 20% ramp.

---

**👤 You:**
> "We have a capacity gap of $2,000,000. How many new AEs do we need if the average full quota is $1,000,000 and turnover is 10%?"

**🤖 AI Agent:**
> You need to hire 2 new AEs to close the gap and 1 additional hire to account for expected turnover.

---

**👤 You:**
> "Calculate the gap between a $5,000,000 growth target and our current $3,500,000 capacity."

**🤖 AI Agent:**
> The capacity gap is $1,500,000, which represents a 42.8% shortfall.


## ❓ FAQ

**Q: How does the tool account for new hires?**
The engine uses ramp schedules to ensure that `get_current_capacity` and hiring forecasts reflect that new AEs contribute only a fraction of their quota during their initial months.

**Q: Can I plan for employee turnover?**
Yes, `forecast_hiring_needs` calculates both the required headcount to close the gap and the replacement headcount needed to cover expected turnover.

**Q: How do I get a monthly hiring schedule?**
You can use the `generate_hiring_timeline` tool by providing your hiring plan and the target month to receive a projected capacity path.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-sales-capacity-planner](https://vinkius.com/ai-agent-connect/enterprise-sales-capacity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Sales Capacity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-sales-capacity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Sales Capacity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-sales-capacity-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
