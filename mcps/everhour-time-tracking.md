# Everhour Time Tracking MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everhour-time-tracking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/everhour-time-tracking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/everhour-time-tracking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to track time, manage projects, and monitor budgets via the Everhour API.

## Description
Integrate **Everhour**, the powerful time tracking and project management software, directly into your AI workflow. Manage your projects and tasks, track real-time time entries and team productivity, monitor project budgets and billing status, and oversee your entire team's workload using natural language.

### What you can do

- **Project Oversight** — List and retrieve detailed information, budgets, and status for all your tracked projects.
- **Time Intelligence** — Monitor team time records, resolving task IDs, durations, and active user timers in real-time.
- **Budget Management** — Access and monitor project budgets, identifying utilization rates and identifying projects at risk of exceeding limits.
- **Productivity Auditing** — Retrieve high-level summaries of recent time entries, task completion, and organizational account health instantly.

### How it works

1. Connect the Everhour integration to your AI assistant.
2. Authorize using your Everhour API Key (found in your account settings).
3. Orchestrate your time tracking and project management strategy through intuitive conversation.

### Who is this for?

- **Project Managers** — Quickly check project budgets and team time entries on the go.
- **Agency Owners** — Research client billing and total hours logged via chat.
- **Operations Teams** — Monitor running timers and organizational productivity metadata instantly.


## Available Tools
- **get_everhour_user_metadata**: Retrieve metadata and profile information for the current Everhour user
- **get_project_detailed_data**: Get detailed settings and budget information for a specific project
- **quick_time_tracking_audit**: Retrieve a high-level summary of recent time entries and active projects
- **get_currently_running_timer**: Retrieve the task and start time for any currently active timer
- **list_billing_clients**: List all clients configured for project billing and invoicing
- **list_tracked_projects**: List all projects managed in your Everhour account
- **list_project_tasks**: List all tasks within a specific project
- **list_organization_team_members**: List all team members and their roles in the organization
- **list_team_time_records**: List time records for the team within a specific date range
- **list_projects_within_budget**: Identify projects that are currently within their assigned time or monetary budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Everhour Time Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects currently over budget."

**🤖 AI Agent:**
> I've identified 2 projects exceeding their budget: 'Website Redesign' (115% utilization) and 'Q1 Marketing Campaign' (102% utilization). Would you like to see the breakdown of hours by team member for the Website Redesign?

---

**👤 You:**
> "Show me the tasks for project 'Mobile App'."

**🤖 AI Agent:**
> The 'Mobile App' project has 12 tasks, including 'User Authentication' (8h logged), 'API Integration' (15h logged), and 'UI/UX Design'. Total time logged for this project is 45 hours. Should I pull the estimated vs. actual time for these tasks?

---

**👤 You:**
> "What is the team productivity summary for this week?"

**🤖 AI Agent:**
> This week, the team has logged a total of 120 hours across 5 active projects. 'John Doe' has logged the most hours (35h), followed by 'Jane Smith' (32h). Average daily productivity is 6 hours per member. Would you like a list of any missing time entries?


## Installation & Usage

To install and use the **Everhour Time Tracking** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everhour-time-tracking](https://vinkius.com/mcp/everhour-time-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
