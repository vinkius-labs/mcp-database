# WorkflowMax MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workflowmax)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/workflowmax-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/workflowmax-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage jobs, clients, and timesheets via WorkflowMax by BlueRock directly from your AI agent.

## Description
Connect your **WorkflowMax by BlueRock** account to any AI agent to automate your job management and time tracking workflows. WorkflowMax provides an all-in-one platform for managing projects, client relations, and billable hours through natural conversation.

### What you can do

- **Job & Project Management** — List all active jobs, fetch detailed metadata, and create or update project records programmatically.
- **Client & Contact Coordination** — Access your customer database, retrieve contact profiles, and manage client relations via natural language.
- **Time Tracking Automation** — Log new timesheet entries for specific tasks and jobs, and monitor recorded hours for better productivity insights.
- **Task & Service Oversight** — Monitor all service tasks available in your system to ensure tasks are assigned and tracked correctly.
- **Operational Intelligence** — Get instant visibility into job statuses and team workloads using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your WorkflowMax Client ID, Client Secret, and Account (Organisation) ID
3. Connect your account via the standard OAuth 2.0 flow
4. Start managing your professional services from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agency Owners** — streamline client management and get real-time job status reports without switching apps.
- **Project Managers** — automate the creation of new jobs and task assignments via natural conversation.
- **Professional Services Teams** — quickly log billable hours and track project progress through simple natural language commands.


## Available Tools
- **create_client_contact**: Requires the client UUID and contact details.

Create a new client contact
- **create_client**: Requires a company or individual name.

Create a new client
- **create_job**: Requires essential details like name, client ID, and start date.

Create a new job
- **create_timesheet**: Requires job UUID, task UUID, and the duration/hours.

Create a new timesheet entry
- **get_client_contact**: Get details for a specific client contact
- **get_client**: Get details for a specific client
- **get_job**: Get details for a specific job
- **list_clients**: List all WorkflowMax clients
- **list_jobs**: Useful for getting an overview of active projects.

List all WorkflowMax jobs
- **list_tasks**: Tasks are the service units that can be assigned to jobs.

List all tasks
- **list_timesheets**: Useful for auditing time logs and work progress.

List timesheet entries
- **update_job**: Update an existing job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WorkflowMax** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs in my WorkflowMax account."

**🤖 AI Agent:**
> I've retrieved 5 active jobs, including 'Website Redesign' (job_123) and 'Tax Audit 2024' (job_456). Would you like to see the recorded timesheets for any of them?

---

**👤 You:**
> "Log 2 hours for task 'Design' on job 'job_123'."

**🤖 AI Agent:**
> Done! I've successfully logged 120 minutes against the 'Design' task for the specified job. The entry is now visible in your WorkflowMax timesheets.


## Installation & Usage

To install and use the **WorkflowMax** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workflowmax](https://vinkius.com/mcp/workflowmax)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
