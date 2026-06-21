# Teamwork Projects MCP Server

Manage projects, tasks, milestones, time entries, and messages via Teamwork API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/teamwork-projects)

## Overview
**Category:** productivity
**Tools Count:** 17

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


## Available Tools
- **create_message**: Body should include title and body content.

Post a new message in a project
- **create_milestone**: Body should include title and deadline date.

Create a new milestone in a project
- **create_project**: Body should include name and optional settings.

Create a new project
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


## Installation & Usage

To install and use the **Teamwork Projects** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teamwork-projects](https://vinkius.com/mcp/teamwork-projects)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
