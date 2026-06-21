# DeskTime MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/desktime)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/desktime-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/desktime-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Understand how your team spends their workday with automatic time tracking, productivity scoring, and project cost analysis.

## Description
Connect your **DeskTime** account to any AI agent and take full control of your workforce management and productivity tracking workflows through natural conversation.

### What you can do

- **Project & Task Orchestration** — List and manage time-tracking projects and individual tasks programmatically to maintain a high-fidelity record of work distribution
- **Team Visibility** — Monitor real-time staff activity, including who is currently online and tracking time, to coordinate team availability and throughput
- **Productivity Intelligence** — Access comprehensive productivity reports and performance metrics for individual employees or the entire company directly through your agent
- **Workflow Automation** — Programmatically create new projects, assign tasks, and mark work as completed to streamline your project management cycle
- **Administrative Oversight** — Retrieve detailed company metadata and employee directories to maintain a perfectly coordinated workforce ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your DeskTime settings (Settings > Integrations)
3. Start managing your team's productivity from Claude, Cursor, or any MCP client

No more manual logging or digging through productivity charts in the dashboard. Your AI acts as your dedicated workforce operations and time-tracking coordinator.

### Who is this for?

- **Project Managers** — instantly retrieve task completion reports and update project statuses using natural language commands
- **Team Leads** — monitor real-time availability and productivity scores without leaving your communication tools
- **HR & Ops Leads** — automate employee data retrieval and monitor company-wide time utilization through simple AI queries


## Available Tools
- **mark_task_completed**: Complete a task
- **create_project**: Add new project
- **create_new_task**: Add task to project
- **remove_project**: Delete a project
- **get_company_info**: Get company details
- **get_employee_performance**: Check employee stats
- **list_online_staff**: Check who is working
- **get_project_details**: Get project info
- **list_employees**: List company employees
- **list_projects**: List DeskTime projects
- **get_productivity_reports**: Check company performance
- **list_project_tasks**: List tasks in project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeskTime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a list of all employees currently tracking time."

**🤖 AI Agent:**
> I've retrieved the online staff list. Currently, 5 employees are tracking time, including @user1 and @user2. Productivity levels are looking healthy across the team.

---

**👤 You:**
> "Check the productivity report for 'last_week'."

**🤖 AI Agent:**
> Scanning reports... Last week, the company average productivity was 84%. Total tracked time: 320 hours. Would you like a breakdown of the top performers?

---

**👤 You:**
> "Create a new task 'Review MCP API' in project ID '123'."

**🤖 AI Agent:**
> Action complete! Task 'Review MCP API' has been successfully created within project 123. Your team can now start tracking time against this specific task.


## Installation & Usage

To install and use the **DeskTime** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/desktime](https://vinkius.com/mcp/desktime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
