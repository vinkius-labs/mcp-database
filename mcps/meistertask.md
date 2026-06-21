# MeisterTask MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meistertask)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Organize team tasks with visual Kanban boards, recurring workflows, and integrations that connect to your favorite tools.

## Description
Connect your **MeisterTask** account to any AI agent and take full control of your agile project orchestration and team productivity through natural conversation. MeisterTask provides a flexible platform for managing project boards, and this integration allows you to retrieve board metadata, create automated task assignments, and monitor real-time team progress directly from your chat interface.

### What you can do

- **Project & Board Orchestration** — List all managed projects and retrieve detailed section (column) metadata programmatically to ensure your team's roadmap is always synchronized.
- **Task Lifecycle Management** — Create, update, and delete tasks with detailed descriptions and assignments directly from the AI interface to maintain high-fidelity workflow automation.
- **Section & Workflow Intelligence** — List all sections within a project and move tasks between them via natural language to drive better team alignment and project transparency.
- **Communication & Comment Control** — Access and monitor task comments to stay informed about team updates and provide synthesized summaries using simple AI commands.
- **Operational Monitoring** — Track system responses and manage user profile metadata to ensure your agile execution is always optimized.

### How it works

1. Subscribe to this server
2. Enter your MeisterTask Access Token (or Personal Access Token) from your developer settings
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the dashboard for task updates. Your AI acts as a dedicated project coordinator or scrum assistant.

### Who is this for?

- **Project Managers & Team Leads** — quickly retrieve project summaries and monitor task health without switching apps.
- **Operations Teams** — automate the creation of recurring tasks and track team capacity via natural conversation.
- **Developers** — integrate real-time project data and board metadata directly within the chat.


## Available Tools
- **create_new_task**: Add new task
- **remove_task**: Delete a task
- **get_api_status**: Check connection
- **get_project_details**: Get board info
- **get_task_details**: Get task info
- **list_all_accessible_tasks**: List all tasks
- **list_task_comments**: Get task history
- **list_task_projects**: List project boards
- **list_project_sections**: List board columns
- **list_section_tasks**: List tasks in section
- **search_tasks_by_query**: Find tasks
- **update_task_info**: Modify a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MeisterTask** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in MeisterTask."

**🤖 AI Agent:**
> I've retrieved your project boards. You have 4 active environments: 'Software Development', 'Marketing Q4', 'Customer Support', and 'Internal HR'. Which one would you like to see sections for?

---

**👤 You:**
> "Create a new task 'Audit API Endpoints' in the 'To Do' section of the 'Software Development' project."

**🤖 AI Agent:**
> Task created! I've added 'Audit API Endpoints' to the 'To Do' section. Would you like me to assign it to a team member or add a description?

---

**👤 You:**
> "Show the latest comments for the 'Fix Login Bug' task."

**🤖 AI Agent:**
> I've retrieved the comments. The last update was from Alice: 'Found the root cause in the session handler, working on a patch' (1 hour ago).


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific task by its ID?**
Yes! Use the `get_task_details` tool with the Task ID. Your agent will respond with complete metadata for the record, including description, assignee, and due date in seconds.

**Q: How do I find my MeisterTask Access Token?**
Log in to MeisterTask, navigate to your **Account** > **API**, and you will find the section to generate a new Personal Access Token for your integration.

**Q: Can I search for tasks by keyword?**
Yes! Use the `search_tasks` tool. Provide your search query, and the agent will retrieve all matching tasks across your accessible project boards instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meistertask](https://vinkius.com/mcp/meistertask)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MeisterTask** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meistertask` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MeisterTask** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meistertask": {
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
