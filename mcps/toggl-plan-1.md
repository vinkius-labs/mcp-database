# Toggl Plan MCP Server

Manage your team's visual timelines, track project phases, and balance workloads securely via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/toggl-plan-1)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Toggl Plan** workspaces to an AI agent entirely bypassing the complex graphical interfaces. Allow your project managers and team leads to directly read, create, and organize workload data, milestones, and daily tasks inside a conversational or command-driven environment.

### What you can do

- **Timeline Oversight** — Search workspaces to list, read, or inspect the metadata details of specific timeline tasks and milestones
- **Project Construction** — Easily list all the active project segments directly on your terminal to know what your team is facing today
- **Task Execution** — Complete the full cycle of task management: Create new nodes on the timeline, update existing entries, or delete deprecated ones through simple instructions
- **Fleet Operations** — Manage human resources by securely listing all registered workspace users to assign workloads correctly
- **Taxonomy Organization** — Check and retrieve current tagging structures to ensure standardized labels

### How it works

1. Subscribe your AI to this component
2. Introduce your specific Toggl Plan authorization credentials (API Token)
3. Query your timeline data or instruct the machine to log hours or schedule new routines fluently

### Who is this for?

- **Project Managers** — Handle timelines, insert tasks, and inspect due dates directly in chat without breaking their daily workflow
- **Resource Planners** — Access user directories and measure scheduled items against operational milestones continuously
- **Software Engineers** — Synchronize technical updates straight to the Toggl timeline without clicking through the official frontend


## Available Tools
- **create_milestone**: Creates a new milestone diamond on the timeline
- **create_timeline_task**: Provide name, start_date, and end_date (YYYY-MM-DD).

Creates a new task/segment on the Toggl Plan timeline
- **delete_timeline_task**: This action is irreversible.

Permanently deletes a task from the timeline
- **get_task_details**: Retrieves details for a specific timeline task
- **get_timeline_view**: Provide since and until dates (YYYY-MM-DD).

Get the visual timeline view from Toggl Plan within a date range
- **list_workspace_members**: Lists all team members in the workspace
- **list_milestones**: Lists all milestones markers on the timeline
- **list_workspace_projects**: Lists all projects in the workspace
- **list_workspace_tags**: Lists all tags used for task categorization
- **update_timeline_task**: Provide updates as a JSON object.

Updates an existing timeline task


## Installation & Usage

To install and use the **Toggl Plan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/toggl-plan-1](https://vinkius.com/mcp/toggl-plan-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
