# Pipeline Velocity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipeline-velocity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate sales pipeline velocity ($/day) and identify which operational metric (opportunities, close rate, or ACV) must improve to hit your revenue targets.

## Description
**Hook:** Your current sales forecast might feel vague. You know you need more revenue, but don't know where the gap is--the funnel size, the win rate, or the deal value.


## Available Tools (3)
- **project_revenue_and_sensitivity**: Also calculates how much revenue would change if each individual variable improved by a given percentage, helping identify which lever has the biggest impact.

Project revenue for a period and analyze sensitivity to variable improvements
- **determine_required_throughput**: Specify primaryMetricToSolveFor as opportunities, close_rate, or sales_cycle.

Determine what operational metric must improve to hit a revenue target
- **calculate_pipeline_velocity**: Requires opportunity count, close rate (0-1), average contract value, and sales cycle length in days.

Calculate sales pipeline velocity in dollars per day


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Velocity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We have 50 active deals, a close rate of 0.25, an ACV of $100,000, and the average sales cycle is 60 days. What is our current daily pipeline velocity?"

**🤖 AI Agent:**
> The calculated daily pipeline velocity is $[TOTAL_VELOCITY]/day. This means your funnel converts potential value at a rate of $X per day.

---

**👤 You:**
> "We need to hit $5,000,000 in the next 90 days. Our current opportunities are 70, close rate is 0.2, and ACV is $80k. What do we need to solve for: opportunities, close_rate, or sales_cycle?"

**🤖 AI Agent:**
> To hit the target of $5M in 90 days, your required daily velocity is $[REQUIRED_DAILY_VELOCITY]/day. Based on current metrics, you must focus on increasing 'opportunities' to reach a count of [NEW_OPPCOUNT] units.

---

**👤 You:**
> "Project our revenue for the next 90 days, assuming we improve our close rate by 15% and keeping everything else constant. What is the total projected impact?"

**🤖 AI Agent:**
> The initial projection over 90 days is $[BASE_REVENUE]. With a 15% improvement in close rate, your new total projected revenue increases by $[IMPACT_AMOUNT], reaching a new high of $[NEW_TOTAL_REVENUE].


## ❓ FAQ

**Q: How do I determine if my current pipeline is growing fast enough to hit a quarterly target?**
Use the `determine_required_throughput` tool. You input your total revenue goal and time period, specifying whether you want to solve for 'opportunities', 'close_rate', or 'sales_cycle'. This tells you exactly what needs to change.

**Q: I need an estimate of my total expected revenue if all things continue as usual for the next 90 days. Which tool handles this?**
The `project_revenue_and_sensitivity` tool is designed for this. It takes your base metrics (opportunity count, close rate, etc.) and projects the total revenue over a specified number of days.

**Q: What is the core calculation for daily sales velocity?**
The `calculate_pipeline_velocity` tool calculates this rate. It takes your total opportunities, close rate, average contract value, and cycle length to give you the speed of revenue realization in dollars per day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipeline-velocity-calculator](https://vinkius.com/mcp/pipeline-velocity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Velocity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-velocity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Velocity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-velocity-calculator": {
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
