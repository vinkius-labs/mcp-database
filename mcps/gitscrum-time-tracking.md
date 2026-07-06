# GitScrum Time Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-time-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track time and budgets via GitScrum — start timers, log hours, analyze productivity, monitor burn-down, and review standup summaries directly from any AI agent.

## Description
### What you can do

- **Live time tracking** — start, stop, and manage timers on any task with one command
- **Manual time logging** — record retroactive time entries with exact start/end timestamps and descriptions
- **Productivity analytics** — access team reports, individual productivity scores, and timeline visualizations
- **Budget monitoring** — check budget burn-down, consumption breakdowns, risk alerts, and project budget health
- **Daily standups** — get automated standup summaries, yesterday's completions, current blockers, and stuck tasks
- **Team insights** — review contributor activity scores, weekly digests, and per-member time breakdowns

### How it works

1. Subscribe to the GitScrum Time Tracking integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Start tracking time conversationally — ask your agent to start a timer, log hours, or review team productivity in Claude, Cursor, or any MCP client

Your agent eliminates the friction of manual time entry and gives you instant visibility into team performance.

### Who is this for?

- **Developers** — start and stop timers without leaving the IDE or opening a browser
- **Team leads** — review standup summaries and identify blockers through natural conversation
- **Project managers** — monitor budget burn-down and track billable hours across projects


## Available Tools (28)
- **budget_overview**: Get project budget overview
- **projects_at_risk**: Get projects at budget risk
- **my_tasks**: Ideal for quickly finding what to track time on.

Get tasks assigned to me across all workspaces
- **standup_blockers**: Get current blockers
- **completed_yesterday**: Get tasks completed yesterday
- **contributors**: Filter by period (week, month, quarter, year).

Get contributor activity summary
- **weekly_digest**: Get weekly activity digest
- **stuck_tasks**: Get stuck tasks
- **standup_summary**: Get daily standup summary
- **team_status**: Get team member status
- **get_task**: Use this to verify a task before starting a timer.

Get task details by UUID
- **list_tasks**: Filter by status (todo, in-progress, done).

List project tasks for time tracking
- **my_today_tasks**: Perfect for daily time tracking workflow.

Get tasks due today
- **get_active_timer**: Only one timer can be active at a time.

Get the currently running timer
- **time_analytics**: Get time tracking analytics
- **delete_time_entry**: Delete a time tracking entry
- **list_time_entries**: List time tracking entries for a project
- **log_manual_time**: Use for retroactive time logging.

Create a manual time entry
- **productivity_report**: Get productivity report
- **time_reports**: Get comprehensive time reports
- **start_timer**: Only one timer can be active at a time. Use stop_timer to end it.

Start a timer on a task
- **stop_timer**: Stop the running timer
- **team_time_report**: Get team time report
- **time_timeline**: Get time entries timeline
- **budget_alerts**: Get budget threshold alerts
- **budget_burndown**: Get budget burn-down chart data
- **budget_consumption**: Get budget consumption breakdown
- **budget_events**: Get budget event log


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum Time Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Start a timer on task WEB-42 in the web-app project."

**🤖 AI Agent:**
> Timer started on WEB-42: 'Implement user authentication' at 10:23 AM. Timer ID: tt-4521. I'll track until you ask me to stop. Say 'stop timer' when you're done, and I'll record the elapsed time automatically.

---

**👤 You:**
> "Give me the standup summary for today."

**🤖 AI Agent:**
> Today's standup: 14 tasks completed yesterday (5 by johndoe, 4 by janedoe, 3 by alexdev, 2 by sarahpm). 8 tasks in progress. 2 blockers flagged: WEB-38 (waiting on API credentials, 3 days blocked) and WEB-45 (design review pending). Participation: 100%. Shall I dig into the blockers?

---

**👤 You:**
> "Which projects are at budget risk?"

**🤖 AI Agent:**
> 2 projects flagged: 1) 'Mobile App v2' — 92% consumed ($46,000 of $50,000), burn rate $2,300/week, estimated overshoot in 5 days. 2) 'API Redesign' — 78% consumed with sprint scope creep detected. Want me to show the burn-down chart or set up budget alerts?


## ❓ FAQ

**Q: Can the agent start and stop timers on tasks without me opening GitScrum?**
Yes! Use `start_timer` with any task UUID to begin tracking, and `stop_timer` to end it. Only one timer can be active at a time. Use `list_tasks` or `my_today_tasks` first to find the task you want to track. The agent handles the complete flow in seconds.

**Q: Can I get a standup summary without attending the meeting?**
Absolutely. Use `standup_summary` for the daily overview, `completed_yesterday` for what the team shipped, `standup_blockers` for current impediments, and `team_status` for per-member breakdown. It's your entire standup in 4 quick queries.

**Q: Can the agent flag projects that are over budget?**
Yes. Use `projects_at_risk` to see all projects approaching or exceeding their budget threshold. Then drill into any project with `budget_overview` for total vs consumed, `budget_burndown` for trend analysis, and `budget_alerts` for active threshold warnings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-time-tracking](https://vinkius.com/mcp/gitscrum-time-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitScrum Time Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitscrum-time-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitScrum Time Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitscrum-time-tracking": {
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
