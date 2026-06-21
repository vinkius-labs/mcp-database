# Workast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage projects, tasks, and team collaboration with AI directly in your workflow.

## Description
Connect your **Workast** account to any AI agent to streamline your project management and task automation. Workast provides a powerful platform for organizing team workflows, tracking deadlines, and managing project backlogs directly within your existing communication tools.

### What you can do

- **Project & Space Orchestration** — Organize your work using Spaces to group related task lists and projects for different teams.
- **Task Lifecycle Management** — Create, list, and update tasks with due dates, priorities, and detailed descriptions.
- **Team Coordination** — List and manage team members to assign responsibilities and monitor project progress programmatically.
- **Metadata Synchronization** — Access team-wide metadata and user profiles to keep your AI workflows aligned with your organization.
- **Real-time Status Updates** — Use natural language to get instant summaries of active spaces and task completion statuses.

### How it works

1. Subscribe to this server
2. Enter your Workast API Token from your account preferences
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — automate the creation and tracking of team tasks via natural conversation.
- **Team Leads** — monitor progress across different spaces and channels without switching apps.
- **Agile Teams** — quickly update task statuses and manage backlogs using simple natural language commands.


## Available Tools (12)
- **create_space**: Create a new space
- **create_task**: Create a new task
- **delete_task**: Delete a task
- **get_account_profile**: Get my profile
- **get_space**: Get space details
- **get_task**: Get task details
- **get_team_info**: Get team details
- **get_user**: Get user details
- **list_spaces**: List all Workast spaces
- **list_tasks**: List tasks in a space
- **list_users**: List team users
- **update_task**: Update a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active spaces in my Workast account."

**🤖 AI Agent:**
> I've retrieved your spaces. You have 4 active environments: 'Project Alpha', 'Design Team', 'Marketing Q4', and 'Customer Support'. Which one should I inspect?

---

**👤 You:**
> "Show me the tasks currently in the 'Design Team' space."

**🤖 AI Agent:**
> Fetching tasks... I've found 6 pending items in the Design Team space. Top tasks include 'Update UI Kit' (Due: tomorrow) and 'Review Logo Drafts'.


## ❓ FAQ

**Q: How do I generate a Workast API Token?**
Log in to Workast, go to your profile icon, select **Preferences** > **API**, and click 'Generate new token' to create your unique access credential.

**Q: What is a 'Space' in Workast?**
A Space is a container for your task lists. It is typically used to organize different projects, client work, or team-specific channels within your workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workast](https://vinkius.com/mcp/workast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workast": {
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
