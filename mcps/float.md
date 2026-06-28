# Float MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/float)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage team scheduling, project allocations, and time off via AI agents with Float.

## Description
Connect your **Float** account to any AI agent and automate your resource management and team scheduling through the Model Context Protocol (MCP). Float is the leading resource planning platform that helps agencies and teams keep track of who is working on what and when. Now, you can manage allocations, check availability, and oversee project timelines directly through natural conversation.

### What you can do

- **Team Scheduling** — List all team members and fetch detailed availability and profile metadata.
- **Project Oversight** — Access active projects, retrieve specific project details, and manage the team members assigned to them.
- **Task Allocations** — Create and list project allocations, assigning specific hours and dates to team members instantly.
- **Time Off Management** — Monitor scheduled vacations, sick leave, and public holidays to ensure accurate capacity planning.
- **Logged Time Analysis** — Retrieve actual hours worked versus scheduled time to track project progress and efficiency.
- **Organization Discovery** — List clients, departments, and account users to maintain full context of your agency's structure.
- **Capacity Planning** — Fetch high-level snapshots of team utilization and task labels (e.g., Design, Development).

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Float Personal Access Token (found in Account Settings > Integrations)
3. Start managing your team resources from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — quickly check if a developer is available for a new task or update a project's timeline.
- **Resource Planners** — get a real-time overview of team capacity and time off via simple AI commands.
- **Agency Directors** — automate the retrieval of logged time reports and client lists for better operational visibility.


## Available Tools (12)
- **get_logged_time**: Get actual hours
- **list_departments**: List departments
- **list_people**: List team members
- **list_project_task_names**: g. Design, Dev).

List task labels
- **list_projects**: List projects
- **list_time_offs**: List time off
- **create_allocation**: Schedule a task
- **get_person**: Get person details
- **get_project**: Get project details
- **list_user_accounts**: List user accounts
- **list_allocations**: List task allocations
- **list_clients**: List clients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Float** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Float and the team members assigned to them."

**🤖 AI Agent:**
> Fetching projects... I found 5 active projects, including 'Website Redesign' (3 members) and 'Mobile App Launch' (5 members). Would you like to see the specific allocations for any of these?

---

**👤 You:**
> "Schedule John Doe for 4 hours a day on the 'Q3 Marketing' project from Monday to Friday."

**🤖 AI Agent:**
> Allocation created! John Doe has been scheduled for 4 hours per day on the 'Q3 Marketing' project for the requested dates. His availability has been updated in Float.

---

**👤 You:**
> "Who is scheduled for time off this month?"

**🤖 AI Agent:**
> Checking time off... This month, Sarah is on vacation from the 10th to the 15th, and Mike has a personal day on the 22nd. Would you like me to check capacity for the rest of the team?


## ❓ FAQ

**Q: How do I check if a team member is available for a specific date range?**
You can use the 'list_allocations' tool to see current schedules. By asking the agent, 'Is John available next week?', it will scan existing task allocations and time off to provide a clear answer.

**Q: Can I assign a person to a project directly through the agent?**
Yes! The 'create_allocation' tool allows you to schedule a person to a project by providing their ID, the project ID, start/end dates, and the number of hours per day.

**Q: How do I see who is currently on vacation?**
Use the 'list_time_offs' tool. It retrieves all scheduled vacations, sick leave, and holidays, giving you an immediate view of who is away from the office.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/float](https://vinkius.com/mcp/float)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Float** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `float` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Float** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "float": {
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
