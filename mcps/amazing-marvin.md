# Amazing Marvin MCP Server

Manage your Amazing Marvin tasks, projects, and time tracking using AI Agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amazing-marvin)

## Overview
**Category:** productivity
**Tools Count:** 9

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


## Installation & Usage

To install and use the **Amazing Marvin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazing-marvin](https://vinkius.com/mcp/amazing-marvin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
