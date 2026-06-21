# Linear (Issue Tracking & PM) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/linear-issue-tracking-pm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/linear-issue-tracking-pm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/linear-issue-tracking-pm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage product development via Linear — track issues, monitor sprint cycles, and audit team projects.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Linear (Issue Tracking & PM)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active issues assigned to me in the 'Engineering' team"

**🤖 AI Agent:**
> I've found 4 active issues for you in Engineering: 1) 'Fix API Timeout' (ENG-101), 2) 'Implement Auth Hook' (ENG-105), 3) 'Update Schema Docs' (ENG-108), and 4) 'Review PR #45' (ENG-112). Which one would you like to update the status for?

---

**👤 You:**
> "Show me the details for issue 'ENG-101'"

**🤖 AI Agent:**
> Issue ENG-101 ('Fix API Timeout'): Priority: Urgent, Status: In Progress, Label: 'Bug'. Description: 'API calls to the /v1/search endpoint are timing out after 30s under heavy load'. It is currently assigned to you and part of the current cycle.

---

**👤 You:**
> "What is the end date for the current sprint cycle?"

**🤖 AI Agent:**
> The current sprint cycle for the Engineering team ends this Friday, March 27th. There are currently 12 active issues in the cycle, with 8 in the 'Todo' or 'In Progress' states. Would you like a list of remaining tasks?


## Installation & Usage

To install and use the **Linear (Issue Tracking & PM)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/linear-issue-tracking-pm](https://vinkius.com/mcp/linear-issue-tracking-pm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
