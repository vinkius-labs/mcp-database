# Amazing Marvin MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazing-marvin)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazing-marvin-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazing-marvin-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Amazing Marvin tasks, projects, and time tracking using AI Agents.

## Description
### What you can do

Integrate the power of Amazing Marvin directly into your favorite AI Agents. This server enables your agents to:
- **Create and Update Tasks**: Quickly add new tasks or modify existing ones without leaving your interface.
- **Organize Projects & Categories**: Create structured categories and projects to keep your workspace tidy.
- **Track Your Time**: Start and stop time trackers directly via AI to maintain perfect logs.
- **Daily Overview**: Retrieve all items scheduled for today so your agent can brief you seamlessly.

### How it works

1. **Get your Token**: Navigate to your Amazing Marvin API settings and copy your unique token.
2. **Connect**: Input the token into your Vinkius environment.
3. **Use the Agent**: Start managing your entire day using natural language!

### Who is this for?

This integration is perfect for founders, developers, and project managers who want to automate their daily workflow, offload task management to AI, and never miss a beat when it comes to time tracking and organizing their Amazing Marvin workspace.


## Available Tools
- **add_category**: Add a new category to Amazing Marvin
- **add_project**: Add a new project to Amazing Marvin
- **add_task**: You can optionally specify a parent category/project ID and a date (YYYY-MM-DD) for when the task is scheduled.

Add a new task to Amazing Marvin
- **get_children**: If no ID is given, it might fetch the root items.

Get tasks and sub-categories inside a category or project
- **get_today_items**: Get tasks scheduled for today in Amazing Marvin
- **mark_done**: Mark a task as completed in Amazing Marvin
- **start_tracking**: Start time tracking for a task in Amazing Marvin
- **stop_tracking**: Stop the currently running time tracker in Amazing Marvin
- **update_task**: You can change its title, scheduled day, or done status.

Update an existing task in Amazing Marvin


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazing Marvin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What do I have scheduled for today in Amazing Marvin?"

**🤖 AI Agent:**
> You have 3 tasks scheduled for today: 1. Reply to emails, 2. Update the staging server, 3. Buy groceries.

---

**👤 You:**
> "Add a new task to call the client and schedule it for tomorrow."

**🤖 AI Agent:**
> I've added the task 'Call the client' and scheduled it for tomorrow.

---

**👤 You:**
> "Start tracking time for the 'Database migration' task."

**🤖 AI Agent:**
> Time tracking has started for the 'Database migration' task.


## Installation & Usage

To install and use the **Amazing Marvin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazing-marvin](https://vinkius.com/mcp/amazing-marvin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
