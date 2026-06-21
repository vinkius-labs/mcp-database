# Teambition MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teambition)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/teambition-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/teambition-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Collaborative project management platform by Alibaba — manage tasks, projects, and team workflows via AI.

## Description
Empower your AI agent to orchestrate your team's productivity with **Teambition**, the leading collaboration platform under Alibaba Group. By connecting Teambition to your agent, you transform complex project tracking and task assignment into a natural conversation. Your agent can instantly list your projects, create new tasks, update statuses, and even browse organization members without you ever touching the web interface. Whether you are managing a software development sprint or a marketing campaign, your agent acts as a real-time project assistant, keeping your workspace organized and your team aligned.

### What you can do

- **Project Management** — List all accessible projects, get detailed info, and monitor overall progress.
- **Task Operations** — Create, update, and track tasks with full support for descriptions, assignees, and due dates.
- **Workflow Visualization** — Browse task groups and stages to understand your Kanban or list-based workflows.
- **Team Coordination** — List project members and organization users to manage assignments effectively.
- **Organization Insights** — Retrieve high-level information about your Teambition organization structure.

### How it works

1. Subscribe to this server
2. Enter your Teambition App ID and App Secret
3. Start managing your projects through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — track development progress, audit task statuses, and align team members through natural language.
- **Software Developers** — manage your assigned tasks and update project progress directly from your AI-powered workspace.
- **Operations Teams** — oversee multiple project workflows and organizational structures through a unified AI interface.
- **Enterprise Leaders** — get real-time insights into organization-wide project activity and team member coordination.


## Available Tools
- **create_task**: Create a new Teambition task
- **get_org_info**: Get organization details
- **get_project**: Get Teambition project details
- **list_members**: List project members
- **list_projects**: List all Teambition projects
- **list_stages**: List stages in a task group
- **list_task_groups**: List task groups in a project
- **list_tasks**: List tasks in a project
- **list_users**: List organization users
- **update_task**: Update an existing Teambition task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teambition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active projects on Teambition."

**🤖 AI Agent:**
> I've retrieved your Teambition projects. You have 4 active projects, including 'Website Redesign' and 'Q2 Marketing Plan'. Which one would you like to explore?

---

**👤 You:**
> "Create a task in project 'Product Launch' titled 'Review landing page copy'."

**🤖 AI Agent:**
> Done! I've created the task 'Review landing page copy' in the 'Product Launch' project. Would you like to assign it to someone or set a due date?

---

**👤 You:**
> "Show me the tasks for project 'Internal Audit'."

**🤖 AI Agent:**
> I've listed the tasks for 'Internal Audit'. There are 8 pending tasks, including 'Inventory check' and 'Compliance review'. Should I filter them by status or assignee?


## Installation & Usage

To install and use the **Teambition** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teambition](https://vinkius.com/mcp/teambition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
