# ONES MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ones)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ones-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ones-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enterprise R&D project management platform — manage tasks, projects, and workflows via AI.

## Description
Empower your AI agent to orchestrate your R&D lifecycle with **ONES**, the leading enterprise project management platform. By connecting ONES to your agent, you transform complex issue tracking, requirement management, and workflow auditing into a natural conversation. Your agent can instantly list your projects, create new tasks, update statuses, and even browse team members without you needing to navigate the comprehensive ONES dashboard. Whether you are following Scrum, Kanban, or Waterfall, your agent acts as a real-time R&D assistant, keeping your projects organized and your team aligned.

### What you can do

- **Project Management** — List all accessible projects and retrieve detailed information about your R&D workspace.
- **Task Operations** — Create, update, and track tasks with full support for summaries, descriptions, and assignees.
- **Workflow Auditing** — Browse project workflows and task types to understand your team's development process.
- **Team Coordination** — List organization members to manage assignments and collaboration effectively.
- **Organization Insights** — Retrieve high-level summaries of your ONES organization activity.

### How it works

1. Subscribe to this server
2. Enter your ONES API Access Token and Organization ID
3. Start managing your R&D projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **R&D Managers** — track development progress, audit task statuses, and monitor team velocity through natural language.
- **Software Engineers** — manage your assigned tasks and update project progress directly from your AI-powered workspace.
- **Product Owners** — monitor requirement fulfillment and release readiness across multiple projects.
- **Enterprise Leaders** — get real-time insights into organization-wide R&D activity and resource allocation.


## Available Tools
- **create_task**: Create a new ONES task
- **get_org_info**: Get organization summary
- **get_project**: Get project details
- **get_task_details**: Get task details
- **list_members**: List organization members
- **list_projects**: List all ONES projects
- **list_task_types**: g., bug, task, story).

List task types
- **list_tasks**: List tasks in a project
- **list_workflows**: List project workflows
- **update_task**: Update an existing ONES task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ONES** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active R&D projects on ONES."

**🤖 AI Agent:**
> I've retrieved your active ONES projects. You have 4 active projects, including 'Core Platform V2' and 'Security Hardening'. Which one would you like to review?

---

**👤 You:**
> "Create a new task in project 'Mobile SDK' titled 'Implement OAuth2 login'."

**🤖 AI Agent:**
> Done! I've created the task 'Implement OAuth2 login' in the 'Mobile SDK' project. Would you like to assign it to someone or add a more detailed description?

---

**👤 You:**
> "Show me the recent activity summary for our organization."

**🤖 AI Agent:**
> I've retrieved the organization summary. In the last 7 days, 150 tasks were created and 120 were completed across 8 projects. Your team velocity remains stable. Would you like a breakdown by project?


## Installation & Usage

To install and use the **ONES** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ones](https://vinkius.com/mcp/ones)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
