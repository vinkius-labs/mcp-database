# Linear (Issue Tracking & PM) MCP Server

Manage product development via Linear — track issues, monitor sprint cycles, and audit team projects.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/linear-issue-tracking-pm)

## Overview
**Category:** loved-by-devs
**Tools Count:** 14

## Description
Connect your **Linear** workspace to any AI agent and take full control of your issue tracking and product development lifecycle through natural conversation.

### What you can do

- **Issue Orchestration** — List and retrieve recent issues from your workspace, including their exact workflow states and assignee tracking directly from your agent
- **Deep Context Inspection** — Pinpoint specific issues to extract full descriptions, assigned labels, and internal priority levels for rapid status updates
- **Project Monitoring** — List all active mapped projects and track their organizational scopes, active state flags, and timeline limits securely
- **Sprint & Cycle Audit** — Monitor current tracking sprint cycle bounds and temporal limits to understand team progress across active iteration loops
- **Team Management** — Enumerate all logical team boundaries and workspace members to route operational assignments and project scopes efficiently
- **Workflow Taxonomy** — Discover global metadata tags and labels used to categorize issues, ensuring your AI agent understands your internal organization rules

### How it works

1. Subscribe to this server
2. Enter your Linear API Key
3. Start managing your product roadmap from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — fetch issue contexts and update task statuses through natural conversation without leaving your IDE
- **Product Managers** — monitor project progress and audit sprint cycles to prepare for weekly syncs and roadmap planning
- **Engineering Leads** — track team assignments and issue distributions across multiple projects to ensure optimized resource allocation


## Available Tools
- **list_teams**: List all logical team segment boundaries mapping workspace access
- **create_issue**: Requires team_id from list_teams.

Create a new issue in a Linear team
- **search_issues**: Returns matching issues with state and assignee context.

Search Linear issues by keyword
- **list_issues**: List recent issues mapped on Linear workspace
- **get_issue**: Get deep context for a specific identified Linear issue tracking limit
- **list_projects**: List all explicit active mapped projects available in the workspace
- **list_cycles**: List current tracking sprint cycle bounds mapping start/end limits
- **list_labels**: List global string metadata tags bounding issue categorization logic
- **list_users**: List all explicitly mapped workspace members validating active access limits
- **get_viewer**: Get active authenticated mapping validating explicit global User boundaries
- **update_issue**: Use list_workflow_states to get valid state IDs for transitions.

Update an existing Linear issue
- **list_workflow_states**: Use state IDs to transition issues via update_issue.

List all workflow states (Backlog, Todo, In Progress, Done, Cancelled)
- **get_project**: Get detailed information for a specific Linear project
- **create_comment**: Comments notify assignees and subscribers.

Add a comment to a Linear issue


## Installation & Usage

To install and use the **Linear (Issue Tracking & PM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linear-issue-tracking-pm](https://vinkius.com/mcp/linear-issue-tracking-pm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
