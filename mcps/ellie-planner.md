# Ellie Planner MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ellie-planner)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ellie-planner-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ellie-planner-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Ellie Planner** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ellie-planner](https://vinkius.com/mcp/ellie-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
