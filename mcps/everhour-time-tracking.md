# Everhour Time Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everhour-time-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to track time, manage projects, and monitor budgets via the Everhour API.

## Description
Integrate **Everhour**, the powerful time tracking and project management software, directly into your AI workflow. Manage your projects and tasks, track real-time time entries and team productivity, monitor project budgets and billing status, and oversee your entire team's workload using natural language.

### What you can do

- **Project Oversight** — List and retrieve detailed information, budgets, and status for all your tracked projects.
- **Time Intelligence** — Monitor team time records, resolving task IDs, durations, and active user timers in real-time.
- **Budget Management** — Access and monitor project budgets, identifying utilization rates and identifying projects at risk of exceeding limits.
- **Productivity Auditing** — Retrieve high-level summaries of recent time entries, task completion, and organizational account health instantly.

### How it works

1. Connect the Everhour integration to your AI assistant.
2. Authorize using your Everhour API Key (found in your account settings).
3. Orchestrate your time tracking and project management strategy through intuitive conversation.

### Who is this for?

- **Project Managers** — Quickly check project budgets and team time entries on the go.
- **Agency Owners** — Research client billing and total hours logged via chat.
- **Operations Teams** — Monitor running timers and organizational productivity metadata instantly.


## Available Tools
- **get_everhour_user_metadata**: Retrieve metadata and profile information for the current Everhour user
- **get_project_detailed_data**: Get detailed settings and budget information for a specific project
- **quick_time_tracking_audit**: Retrieve a high-level summary of recent time entries and active projects
- **get_currently_running_timer**: Retrieve the task and start time for any currently active timer
- **list_billing_clients**: List all clients configured for project billing and invoicing
- **list_tracked_projects**: List all projects managed in your Everhour account
- **list_project_tasks**: List all tasks within a specific project
- **list_organization_team_members**: List all team members and their roles in the organization
- **list_team_time_records**: List time records for the team within a specific date range
- **list_projects_within_budget**: Identify projects that are currently within their assigned time or monetary budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Everhour Time Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects currently over budget."

**🤖 AI Agent:**
> I've identified 2 projects exceeding their budget: 'Website Redesign' (115% utilization) and 'Q1 Marketing Campaign' (102% utilization). Would you like to see the breakdown of hours by team member for the Website Redesign?

---

**👤 You:**
> "Show me the tasks for project 'Mobile App'."

**🤖 AI Agent:**
> The 'Mobile App' project has 12 tasks, including 'User Authentication' (8h logged), 'API Integration' (15h logged), and 'UI/UX Design'. Total time logged for this project is 45 hours. Should I pull the estimated vs. actual time for these tasks?

---

**👤 You:**
> "What is the team productivity summary for this week?"

**🤖 AI Agent:**
> This week, the team has logged a total of 120 hours across 5 active projects. 'John Doe' has logged the most hours (35h), followed by 'Jane Smith' (32h). Average daily productivity is 6 hours per member. Would you like a list of any missing time entries?


## ❓ FAQ

**Q: How do I get an Everhour API Key?**
Log in to your Everhour account, navigate to your user profile settings (top right), and click on **API**. You can find or generate your unique API Key there.

**Q: Can the agent start a new timer?**
This integration currently focuses on listing and auditing projects, tasks, and time entries. Starting or stopping live timers should be performed via the Everhour browser extension or mobile app.

**Q: Does the integration show real-time budget usage?**
Yes, you can use the list_projects_within_budget tool to retrieve current budget utilization rates and identify projects that are approaching their limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everhour-time-tracking](https://vinkius.com/mcp/everhour-time-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Everhour Time Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `everhour-time-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Everhour Time Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "everhour-time-tracking": {
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
