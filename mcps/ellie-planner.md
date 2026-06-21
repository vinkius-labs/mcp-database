# Ellie Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ellie-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan projects visually with AI-assisted task breakdowns, timelines, and team coordination that adapts as your work evolves.

## Description
Connect your **Ellie Planner** account to any AI agent and take full control of your daily productivity and time-blocking workflows through natural conversation.

### What you can do

- **Task Orchestration** — Create and manage daily tasks and Brain Dump items programmatically, including retrieving detailed metadata and status
- **Productivity Lifecycle** — Track your progress by marking tasks as completed and updating priorities or dates directly through your agent
- **Categorical Intelligence** — Organize your tasks using account-wide labels and custom lists to maintain a high-fidelity productivity structure
- **Workflow Automation** — Programmatically update or delete tasks to keep your daily plan aligned with your real-time priorities
- **Dashboard Visibility** — Access your complete directory of task lists and labels to ensure every thought is perfectly categorized

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from Ellie Planner settings (Enable 'Toggle power features')
3. Start managing your daily productivity from Claude, Cursor, or any MCP client

No more manual toggling between browser tabs to check your todo list. Your AI acts as your dedicated personal assistant and productivity coordinator.

### Who is this for?

- **Productivity Enthusiasts** — instantly register new ideas into your brain dump and organize your day using natural language
- **Busy Professionals** — update task statuses and check-in on daily goals without leaving your creative workspace
- **Developers** — integrate personal task management and time-blocking into custom internal tools through simple AI queries


## Available Tools (8)
- **complete_task**: Mark a task as completed
- **create_task**: Provide title and optionally date/labels.

Create a new task
- **delete_task**: Delete a task
- **get_task**: Get details of a specific task
- **list_labels**: List all task labels
- **list_lists**: List all task lists
- **list_tasks**: List all tasks
- **update_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ellie Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current tasks for today in Ellie Planner."

**🤖 AI Agent:**
> I've retrieved your tasks for today. You have 5 active items, including 'Finish API Design' and 'Team Meeting'. Which one should we update or mark as completed?

---

**👤 You:**
> "Create a task 'Research MCP Servers' in my Brain Dump."

**🤖 AI Agent:**
> Done! I've added 'Research MCP Servers' to your Brain Dump list. It's now ready for you to schedule or prioritize later.

---

**👤 You:**
> "Mark task ID 't_123' as completed."

**🤖 AI Agent:**
> Action complete! Task t_123 has been successfully marked as completed in your Ellie Planner. Your progress is now updated on the dashboard.


## ❓ FAQ

**Q: How do I find my API Token?**
Log in to your account, go to Settings, enable the 'Toggle power features' option, and you will see the API Token field.

**Q: Is a Pro plan required?**
Yes, API access and automation features are exclusively available for Ellie Planner Pro subscribers.

**Q: Can the agent manage my labels?**
The agent can list your labels using the `list_labels` tool. To create or edit labels, please use the Ellie Planner web application.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ellie-planner](https://vinkius.com/mcp/ellie-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ellie Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ellie-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ellie Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ellie-planner": {
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
