# Job Search Weekly Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/job-search-weekly-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform job targets and availability into a structured weekly execution plan.

## Description
This MCP server acts as an intelligent scheduling engine for job seekers. It connects your job targets and deadlines with your actual availability to create a balanced weekly plan. You can use `list_job_targets` to see your pending tasks, `get_user_availability` to check your time constraints, and `generate_weekly_schedule` to build a plan using strategies like 'deadline_first' or 'even_spread'. It also includes `validate_plan_feasibility` to ensure your schedule respects all time and deadline constraints.


## Available Tools (4)
- **generate_weekly_schedule**: Generates a structured plan by allocating tasks to available time slots
- **get_user_availability**: Retrieves the total number of hours the user has available for job search activities in the current week
- **list_job_targets**: Retrieves all active job targets, including their associated tasks and deadlines
- **validate_plan_feasibility**: Checks if a proposed or existing schedule is logically sound and within capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Job Search Weekly Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a weekly plan for next Monday using the deadline_first strategy."

**🤖 AI Agent:**
> Your schedule for the week starting 2024-05-20 is ready. I have prioritized your application for Google due on Wednesday and your networking task for Monday.

---

**👤 You:**
> "How many hours do I have available for job searching this week?"

**🤖 AI Agent:**
> You have 25 hours available this week, with a daily breakdown of 5 hours from Monday to Friday.

---

**👤 You:**
> "Is my current schedule feasible given my 15 available hours?"

**🤖 AI Agent:**
> No, the plan is not feasible because the total duration of scheduled tasks (18 hours) exceeds your available 15 hours.


## ❓ FAQ

**Q: How does the scheduling optimization work?**
You can choose between 'deadline_first' to prioritize urgent tasks or 'even_spread' to distribute your workload more evenly across the week.

**Q: Can I verify if my plan is realistic?**
Yes, you can use the `validate_plan_feasibility` tool to check if your schedule respects your available hours and task deadlines.

**Q: How do I see my current job applications?**
Use the `list_job_targets` tool to retrieve all active job targets, including their associated tasks and deadlines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/job-search-weekly-planner](https://vinkius.com/en/ai-agent-connect/job-search-weekly-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Job Search Weekly Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `job-search-weekly-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Job Search Weekly Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "job-search-weekly-planner": {
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
