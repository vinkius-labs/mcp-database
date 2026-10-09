# Team Capacity Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/team-capacity-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forecast deliverable capacity by reconciling availability, holidays, and task dependencies.

## Description
This MCP server provides a specialized forecasting engine to calculate how much work a team can actually complete. It reconciles available personnel hours, scheduled holidays, and task dependencies against a specific utilization target. Use `getTeamAvailability` to find raw capacity, `calculateUtilizedCapacity` to apply efficiency targets, `forecastTaskCompletion` to predict delivery dates, and `analyzeCapacityGap` to identify workload mismatches.


## Available Tools (4)
- **analyzeCapacityGap**: Identifies if there is a mismatch between the effort required for a backlog and the team's actual capacity
- **calculateUtilizedCapacity**: Determines the actual productive capacity after applying the utilization target
- **getTeamAvailability**: Calculates total hours available for a set of team members in a given period
- **forecastTaskCompletion**: Predicts when a specific set of tasks can be completed given current capacity and dependencies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Team Capacity Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many hours does the engineering team have available from 2024-06-01 to 2024-06-30?"

**🤖 AI Agent:**
> The engineering team has a total of 480 available hours for the period of June 2024.

---

**👤 You:**
> "If I have 100 available hours and a utilization target of 0.75, how many productive hours do I have?"

**🤖 AI Agent:**
> You have 75 productive hours available.

---

**👤 You:**
> "Will the current backlog of tasks be completed by the end of the month if we have 40 productive hours available?"

**🤖 AI Agent:**
> No, there is a capacity gap of 15 hours, meaning the current workload exceeds the team's capacity for this period.


## ❓ FAQ

**Q: How is available capacity calculated?**
Available capacity is calculated by taking the standard working hours of team members and subtracting any scheduled holidays or personal leave within the specified date range.

**Q: What is a utilization target?**
A utilization target is a multiplier (e.g., 0.8 for 80%) that accounts for non-task time like meetings and administrative work, converting raw available hours into productive hours.

**Q: Can I forecast specific task completion dates?**
Yes, you can use the `forecastTaskCompletion` tool to predict when a set of tasks will be finished, taking into account task dependencies and team efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/team-capacity-forecast](https://vinkius.com/en/ai-agent-connect/team-capacity-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Team Capacity Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `team-capacity-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Team Capacity Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "team-capacity-forecast": {
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
