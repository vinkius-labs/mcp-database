# Study Schedule Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/study-schedule-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate personalized study schedules based on subject difficulty and available time.

## Description
The Study Schedule Generator is an automated planning engine that creates customized study itineraries. By analyzing subjects, their difficulty levels, and your priority, the tool distributes available study hours proportionally across your timeline. It respects daily availability limits and mandatory rest days to ensure a balanced and realistic plan. Use `generate_weekly_plan` to see your day-by-day breakdown or `get_schedule_overview` for a high-level summary.


## Available Tools (4)
- **get_subject_distribution**: Get the subject importance distribution
- **check_feasibility**: Check if the study plan is feasible
- **get_schedule_overview**: Get a summary of the study schedule
- **generate_weekly_plan**: Generate a detailed weekly study plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Study Schedule Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a study plan for Math (difficulty 3, importance 2) and History (difficulty 1, importance 1) for 7 days, with 2 hours available daily on weekdays."

**🤖 AI Agent:**
> Week 1:
- Monday: Math (1.4h), History (0.6h)
- Tuesday: Math (1.4h), History (0.6h)
- Wednesday: Math (1.4h), History (0.6h)...

---

**👤 You:**
> "Show me the summary of my study plan for 14 days."

**🤖 AI Agent:**
> Total Study Hours: 28
Subject Count: 3
Period Weeks: 2

---

**👤 You:**
> "How much effort am I putting into Physics?"

**🤖 AI Agent:**
> Physics represents 40% of your total study time, with a total allocation of 12 hours.


## ❓ FAQ

**Q: How is the study time distributed among subjects?**
The engine calculates a weight for each subject based on its difficulty and importance, then allocates available hours proportionally to that weight.

**Q: Can I set specific days as rest days?**
Yes, you can provide an array of day indices (0-6) to ensure no study sessions are scheduled on those days.

**Q: What happens if my exam is very soon?**
The `check_feasibility` tool can help you determine if your current workload is manageable given the remaining days until your exam.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/study-schedule-generator](https://vinkius.com/mcp/study-schedule-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Study Schedule Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `study-schedule-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Study Schedule Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "study-schedule-generator": {
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
