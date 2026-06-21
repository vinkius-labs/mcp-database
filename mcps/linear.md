# Linear MCP Server

Streamline issue tracking and project management via Linear — list teams, query issues, create comments and inspect cycles directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/linear)

## Overview
**Category:** loved-by-devs
**Tools Count:** 12

## Description
Connect your **Linear** workspace to any AI agent and take full control of your issue tracking and sprint workflows through natural conversation.

### What you can do

- **User & Team Discovery** — Retrieve the authenticated user profile and list all teams configured in your Linear workspace
- **Issue Management** — List, search, inspect and create issues with full metadata including assignees, labels, priority and state
- **Project Oversight** — Browse all active projects, view their status and drill into specific project details by ID
- **Comments & Collaboration** — Add comments to issues to keep your team context aligned without switching to the Linear app
- **Cycle Tracking** — List all sprint cycles for any team, including start/end dates and completion progress
- **Label Organization** — View all issue labels used for categorization across teams

### How it works

1. Subscribe to this server
2. Enter your Linear Personal API Key
3. Start managing your sprints from Claude, Cursor, or any MCP-compatible client

No more tab-switching to check issue status or hunt for the right assignee. Your AI acts as an on-demand engineering manager.

### Who is this for?

- **Engineering Managers** — instantly pull issue summaries, check cycle progress and audit sprint health without opening Linear
- **Developers** — create and update issues, add comments and check assignees directly from your IDE
- **Product Teams** — monitor project statuses and search across issues to understand feature scope and blockage


## Available Tools
- **create_comment**: The body supports Linear Markdown format including @mentions and ~~strikethrough~~.

Add a comment to a Linear issue
- **create_issue**: Requires the team ID and issue title. Optionally set description, assignee, priority (0=No priority, 1=Urgent, 2=High, 3=Normal, 4=Low) and label IDs.

Create a new Linear issue
- **list_cycles**: Each cycle has a number, name, start date, end date and completion progress percentage.

List Linear cycles (sprints) for a team
- **get_issue**: Use the issue ID (UUID) or the human-readable identifier (e.g. TEAM-123).

Get full details for a Linear issue
- **get_project**: Get details for a specific Linear project
- **list_issues**: Optionally filter by team ID to get issues for a specific team only.

List Linear issues
- **list_labels**: Optionally filter by team ID. Each label has a name, color and optional description.

List Linear issue labels
- **list_projects**: Projects group issues across multiple teams. Use optional limit to control how many results to fetch.

List Linear projects
- **search_issues**: Optionally filter results to a specific team. Returns issues with identifier, title, state, priority, assignee and URL.

Search Linear issues by text
- **list_teams**: Each team has a unique ID, name, key prefix and optional description. Use this to discover teams before querying their issues or cycles.

List all Linear teams
- **update_issue**: Provide the issue ID (UUID) and only the fields you want to change.

Update an existing Linear issue
- **get_viewer**: Useful to verify which account the API token belongs to.

Get current authenticated Linear user details


## Installation & Usage

To install and use the **Linear** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linear](https://vinkius.com/mcp/linear)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
