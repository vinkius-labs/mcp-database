# Nifty MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nifty)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Combine tasks, timelines, docs, and chat in one project management workspace that replaces multiple tools at once.

## Description
Connect your **Nifty** account to any AI agent and take full control of your project orchestration and workflow management through natural conversation. Nifty provides a comprehensive project management platform, and this integration allows you to retrieve project metadata, create automated task assignments, and monitor milestone progress directly from your chat interface.

### What you can do

- **Project & Portfolio Orchestration** — List all managed projects and retrieve detailed metadata programmatically to ensure your team's roadmap is always synchronized.
- **Task Lifecycle Management** — Create, update, and complete tasks directly from the AI interface to maintain high-fidelity workflow automation.
- **Milestone & Sprint Intelligence** — Access and monitor project milestones via natural language to drive better team alignment and deadline transparency.
- **Portfolio Monitoring** — Access and monitor your project portfolios and retrieve status metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and manage user profile metadata to ensure your project operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Nifty Access Token from your app settings
3. Start managing your projects from Claude, Cursor, or any MCP-compatible client

No more manual status checking or context switching. Your AI acts as a dedicated project coordinator or agile lead.

### Who is this for?

- **Project Managers & Product Leads** — quickly retrieve project summaries and monitor task health without switching apps.
- **Agile Teams** — automate the creation of tasks and track milestone completion via natural conversation.
- **Operations Teams** — streamline the retrieval of portfolio metadata and monitor organizational health directly within the chat.


## Available Tools (12)
- **mark_task_as_complete**: Finish a task
- **create_project_milestone**: Add new milestone
- **create_new_task**: Add new task
- **get_api_status**: Check connection
- **get_project_details**: Get board info
- **get_task_info**: Get task details
- **list_project_milestones**: List project phases
- **list_organization_portfolios**: List portfolios
- **list_active_projects**: List project boards
- **list_workflow_tasks**: List project tasks
- **search_all_tasks**: Find tasks
- **update_task_metadata**: Modify a task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nifty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Nifty."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active environments: 'Website Redesign', 'Mobile App Launch', and 'Marketing Q4'. Which one would you like to see the task list for?

---

**👤 You:**
> "Create a new task 'Finalize SEO Audit' in the 'Website Redesign' project."

**🤖 AI Agent:**
> Task created! I've added 'Finalize SEO Audit' to the 'Website Redesign' project. Would you like me to assign it to someone?

---

**👤 You:**
> "Show me the milestones for the 'Mobile App Launch' project."

**🤖 AI Agent:**
> I've retrieved the milestones. You have 2 key phases: 'Design Freeze' (Due: Oct 30) and 'Beta Release' (Due: Nov 15). Shall I check the tasks for either of these?


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific task by its ID?**
Yes! Use the `get_task` tool with the Task ID. Your agent will respond with complete metadata for the record, including assignee details, current status, and due dates in seconds.

**Q: How do I find my Nifty Access Token?**
Log in to your Nifty account (Business Plan or above required), navigate to **App Center** > **Integrate with API**, and you will find your unique secret token there.

**Q: Can I use the AI to mark a milestone as complete?**
The current MCP implementation allows you to monitor milestones and manage tasks. To update a milestone status, we recommend using the Nifty dashboard while we expand tool capabilities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nifty](https://vinkius.com/mcp/nifty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nifty** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nifty` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nifty** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nifty": {
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
