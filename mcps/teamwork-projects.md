# Teamwork Projects MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teamwork-projects)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage projects, tasks, milestones, time entries, and messages via Teamwork API.

## Description
Connect **Teamwork** to any AI agent and manage your project delivery platform — create and track tasks, manage milestones, log time, post messages, and monitor project progress through natural conversation.

### What you can do
- **Project Management** — List and create projects for organizing work
- **Task Management** — Create, update, and delete tasks with assignees and due dates
- **Milestones** — Track project milestones and deadlines
- **Time Tracking** — Log and review time entries against projects
- **Messages** — Post announcements and discussions in projects
- **Files** — List and access project files and attachments

### How it works
1. Subscribe to this server
2. Enter your Teamwork site name and Access Token
3. Start managing projects from Claude, Cursor, or any MCP-compatible client

Teamwork is a comprehensive project management platform used by agencies and professional services teams to deliver work on time and on budget.

### Who is this for?
- **Project Managers** — Create and track work items without opening the web app
- **Team Leads** — Monitor project activity and add messages for team coordination
- **Operations Teams** — Log time entries and manage milestones across multiple projects


## Available Tools (17)
- **create_task**: Body should include content, tasklist_id, assignee_ids, and due dates.

Create a new task
- **create_time_entry**: Body should include description, duration, and date.

Log a new time entry
- **delete_task**: Delete a task
- **list_files**: List all files in a project
- **get_project**: Get details of a specific project
- **get_task**: Get details of a specific task
- **get_current_user**: Use this to verify connection and identify your user ID.

Get the authenticated user profile
- **list_messages**: List all messages in a project
- **list_milestones**: List all milestones in a project
- **list_projects**: Use project IDs to query tasks, milestones, and other resources within specific projects.

List all projects accessible to the user
- **list_tasklists**: Use task list IDs to query specific tasks.

List all task lists in a project
- **list_tasks**: List all tasks in a project
- **list_time_entries**: List all time entries in a project
- **update_task**: Update an existing task
- **create_message**: Body should include title and body content.

Post a new message in a project
- **create_milestone**: Body should include title and deadline date.

Create a new milestone in a project
- **create_project**: Body should include name and optional settings.

Create a new project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teamwork Projects** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my projects."

**🤖 AI Agent:**
> Found 4 projects: 1. Website Redesign. 2. Mobile App Launch. 3. Q1 Marketing Campaign. 4. Client Onboarding.

---

**👤 You:**
> "List all tasks in project 12345."

**🤖 AI Agent:**
> Found 12 tasks: 1. Design Homepage (Due: 2025-04-15). 2. Update API Docs. 3. Fix Login Bug. 4. Launch Campaign.

---

**👤 You:**
> "Create a milestone 'Phase 1 Complete' with deadline 2025-05-01 in project 12345."

**🤖 AI Agent:**
> Milestone created successfully! 'Phase 1 Complete' added to project 12345 with deadline 2025-05-01.


## ❓ FAQ

**Q: How do I get my Teamwork Access Token?**
Log in to Teamwork, go to your Profile picture > My Profile > Developer, and generate a Personal Access Token.

**Q: Can I create tasks with assignees?**
Yes! Use the create_task action with a JSON body that includes content, tasklist_id, and responsible-party-ids for assignment.

**Q: Can I log time against a project?**
Yes! Use the create_time_entry action with a JSON body that includes description, duration (in minutes or seconds), and date.

**Q: Can I retrieve project milestones?**
Yes! Use the list_milestones action to get all project milestones and their deadlines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teamwork-projects](https://vinkius.com/mcp/teamwork-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Teamwork Projects** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `teamwork-projects` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Teamwork Projects** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teamwork-projects": {
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
