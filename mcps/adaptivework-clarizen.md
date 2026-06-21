# AdaptiveWork (Clarizen) MCP Server

Enterprise project management — manage projects, tasks, resources, and portfolios via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/adaptivework-clarizen)

## Overview
**Category:** productivity
**Tools Count:** 6

## Description
Connect your **AdaptiveWork (formerly Clarizen)** account to your AI agent to unlock enterprise-grade project and portfolio management. From tracking high-level project health to creating granular tasks and managing resource availability, your agent handles complex workflows through natural conversation.

### What you can do

- **Project Portfolio Management** — List and audit active projects, check health statuses, and retrieve executive summaries
- **Task Orchestration** — Create, assign, and update tasks across your project structure to ensure team alignment
- **Resource Insights** — List organization users and check assignments to optimize team capacity
- **Advanced Querying (CZQL)** — Run custom Clarizen Query Language commands to retrieve specific data subsets for reporting
- **Portfolio Health** — Quickly identify project bottlenecks or overdue milestones directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AdaptiveWork API Key and Server URL
3. Start managing your enterprise projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — automate task creation and status reporting for large-scale initiatives
- **PMO Leaders** — audit portfolio health and resource utilization across departments
- **Business Analysts** — retrieve project data for financial reporting and performance analysis
- **Team Leads** — quickly update task progress and check team assignments without dashboard fatigue


## Available Tools
- **list_tasks**: Requires the Project ID.

Retrieve the active task list associated with a specific project container ID
- **list_projects**: Can filter by state or status in the tool response natively.

Retrieve a list of active projects managed within the AdaptiveWork organization
- **get_project_details**: Requires the Project ID.

Retrieve detailed metadata and progress metrics for a specific AdaptiveWork project
- **create_task**: You must provide a task name and its parent ID.

Add a new granular task to a project or parent task structure in AdaptiveWork
- **list_users**: Retrieve the list of active organization users in AdaptiveWork to check resource assignments
- **run_query**: Requires valid CZQL syntax.

Execute advanced Clarizen Query Language (CZQL) commands for custom data retrieval


## Installation & Usage

To install and use the **AdaptiveWork (Clarizen)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adaptivework-clarizen](https://vinkius.com/mcp/adaptivework-clarizen)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
