# GitScrum Sprints MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-sprints)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan and track sprints via GitScrum — manage sprint cycles, monitor KPIs, review burndown charts, and organize user stories and epics from any AI agent.

## Description
### What you can do

- **Sprint lifecycle** — create, update, delete, and inspect sprints with precise date ranges and configurations
- **Performance analytics** — access sprint KPIs, detailed statistics, progress tracking, and velocity metrics in real-time
- **Visual reports** — retrieve burndown, burnup, performance, and distribution chart data for any sprint
- **Backlog management** — list and create user stories, browse epics, and view tasks filtered by sprint
- **Cross-workspace visibility** — list sprints across all workspaces for portfolio-level oversight

### How it works

1. Subscribe to the GitScrum Sprints integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Ask your agent to review sprint progress, analyze velocity trends, or plan the next iteration — works in Claude, Cursor, and any MCP client

Your agent delivers sprint analytics and agile insights without requiring manual dashboard navigation.

### Who is this for?

- **Scrum masters** — review sprint KPIs and progress during standups and retrospectives
- **Engineering managers** — track velocity trends and team throughput across sprints
- **Product owners** — manage user stories and epics while monitoring delivery cadence


## Available Tools (15)
- **all_sprints**: List sprints across all workspaces
- **create_user_story**: Create a user story
- **list_epics**: List epics in a project
- **create_sprint**: Create a new sprint
- **get_sprint**: Get sprint details
- **sprint_kpis**: Get sprint KPIs
- **list_sprints**: List sprints in a project
- **sprint_metrics**: Get detailed sprint metrics
- **sprint_progress**: Get current sprint progress
- **sprint_reports**: Resource: burndown, burnup, performance, types, efforts, member_distribution, task, type_distribution.

Get sprint reports with charts
- **sprint_stats**: Get sprint statistics
- **update_sprint**: Update an existing sprint
- **get_task**: Get task details by UUID
- **list_tasks**: Use the sprint_slug filter to see only tasks belonging to a specific sprint. Filter by status (todo, in-progress, done).

List tasks in a project, optionally filtered by sprint
- **list_user_stories**: List user stories in a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum Sprints** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's the progress of our current sprint in the web-app project?"

**🤖 AI Agent:**
> Sprint 'Sprint 14 — Auth Module' is at 68% completion: 17 of 25 tasks done, 5 in progress, 3 in backlog. Velocity is tracking above average at 34 story points. The sprint ends in 4 days. Shall I show you the burndown chart or the remaining in-progress tasks?

---

**👤 You:**
> "Create a new sprint 'Sprint 15 — Payments' from April 14 to April 28."

**🤖 AI Agent:**
> Sprint created! 'Sprint 15 — Payments' runs from 2026-04-14 to 2026-04-28 (2-week cycle). The sprint is empty — would you like me to list the backlog tasks to assign into it, or create user stories for the payments feature?

---

**👤 You:**
> "Show me the velocity metrics for the last completed sprint."

**🤖 AI Agent:**
> Sprint 13 metrics: velocity of 31 story points (vs 28 average), throughput of 22 tasks completed, cycle time averaging 2.1 days per task. The team improved 11% over Sprint 12. Member distribution: johndoe (12 tasks), janedoe (7), alexdev (3). Want me to compare with earlier sprints?


## ❓ FAQ

**Q: Can my AI agent show me the burndown chart data for the current sprint?**
Yes! Use `sprint_reports` with the resource set to 'burndown'. Your agent returns the ideal versus actual burn-down data points, so you can visualize or analyze sprint health instantly. You can also request 'burnup', 'performance', or 'member_distribution' reports.

**Q: Can I see what tasks are in a specific sprint?**
Absolutely. Use `list_tasks` with the `sprint_slug` filter to see only tasks belonging to that sprint. You can further filter by status (todo, in-progress, done) to focus on what matters. Then use `get_task` to drill into any specific task for full details.

**Q: Does this integration support sprint velocity and metrics tracking?**
Yes. Use `sprint_metrics` for detailed velocity, throughput, and efficiency data. Combined with `sprint_kpis` for high-level indicators and `sprint_stats` for task distribution analysis, you get a complete performance picture across any sprint.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-sprints](https://vinkius.com/mcp/gitscrum-sprints)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitScrum Sprints** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitscrum-sprints` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitScrum Sprints** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitscrum-sprints": {
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
