# Weekly Goal Progress MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weekly-goal-progress)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and predict weekly goal completion and progress velocity.

## Description
This MCP server provides tools to monitor how well you are meeting your weekly objectives. You can check the exact completion percentage for a specific goal using `get_weekly_completion`, predict if you will finish a goal on time with `get_goal_velocity`, or get a high-level overview of all active goals via `list_weekly_status_summary`. It also allows you to review historical progress with `get_goal_history` to see how your performance has evolved over time.


## Available Tools (4)
- **list_weekly_status_summary**: Summarize overall progress for all goals in a specific week
- **get_goal_history**: Retrieve historical weekly completion percentages for a goal
- **get_goal_velocity**: Predict if a goal will be finished by the end of the week based on current velocity
- **get_weekly_completion**: Get the percentage of completion for a specific goal this week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Goal Progress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my completion percentage for goal ID 123 this week?"

**🤖 AI Agent:**
> Your completion percentage for goal 123 is 75%.

---

**👤 You:**
> "Will I finish my goal 456 by the end of this week?"

**🤖 AI Agent:**
> Based on your current velocity, you are projected to reach 100% completion with a high probability.

---

**👤 You:**
> "Give me a summary of all my goals for week 42."

**🤖 AI Agent:**
> For week 42, you have 5 active goals with an average completion rate of 60%.


## ❓ FAQ

**Q: How do I check if I will finish my goal this week?**
You can use the `get_goal_velocity` tool to see your projected weekly total and the probability of hitting your target.

**Q: Can I see my progress from previous weeks?**
Yes, the `get_goal_history` tool provides snapshots of your completion percentages from past weeks.

**Q: How is my overall progress for the week?**
Use `list_weekly_status_summary` to get a summary of all active goals, including the average completion rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weekly-goal-progress](https://vinkius.com/en/ai-agent-connect/weekly-goal-progress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Goal Progress** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-goal-progress` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Goal Progress** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-goal-progress": {
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
