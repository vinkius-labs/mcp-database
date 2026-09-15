# Sprint Velocity Trend MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sprint-velocity-trend)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Analyzes historical sprint performance to forecast capacity and identify velocity patterns.

## Description
This MCP server provides advanced analytics for agile teams to monitor and predict their throughput. By connecting to Vinkius Edge, AI agents can use tools like `get_velocity_summary` to assess efficiency trends, `forecast_future_capacity` to project upcoming work limits, and `analyze_scope_impact` to measure the effect of unplanned work. It also includes `calculate_normalized_velocity` to ensure fair comparisons when team sizes change over time.


## Available Tools (4)
- **analyze_scope_impact**: Evaluates how unplanned work (scope creep) is affecting the team's ability to meet commitments
- **calculate_normalized_velocity**: Adjusts historical velocity to account for changes in team size
- **forecast_future_capacity**: Predicts how much work the team can realistically take on in upcoming sprints
- **get_velocity_summary**: Provides a high-level overview of historical performance and current efficiency trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sprint Velocity Trend** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current velocity trend based on these completed points: [20, 22, 25, 28] and a team size of 5?"

**🤖 AI Agent:**
> Your team is showing an improving trend with an average velocity of 23.75 story points.

---

**👤 You:**
> "Predict our capacity for the next sprint. We have completed [30, 35, 32] points, a team of 6, and we planned for 35 points."

**🤖 AI Agent:**
> The projected velocity is 32.33 story points, leaving a capacity buffer of 2.67 points.

---

**👤 You:**
> "How much scope creep did we have if we planned 40 points but only completed 30, 35, and 32 in recent sprints?"

**🤖 AI Agent:**
> The analysis shows a significant deviation between planned and completed work, indicating high instability in recent sprints.


## ❓ FAQ

**Q: How does this tool help with sprint planning?**
It provides data-driven forecasts. For example, using `forecast_future_capacity` allows an agent to suggest a realistic workload based on your team's historical performance and current size.

**Q: Can I account for changes in team size?**
Yes, the `calculate_normalized_velocity` tool adjusts historical data to account for team scaling, ensuring your velocity trends remain accurate even as the team grows or shrinks.

**Q: How is scope creep measured?**
The `analyze_scope_impact` tool compares planned points against completed points to calculate the creep percentage and stability index of your sprints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sprint-velocity-trend](https://vinkius.com/en/ai-agent-connect/sprint-velocity-trend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sprint Velocity Trend** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sprint-velocity-trend` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sprint Velocity Trend** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sprint-velocity-trend": {
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
