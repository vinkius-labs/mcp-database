# Productive.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/productiveio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/productiveio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/productiveio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Run your agency with project management, resource planning, budgeting, and profitability tracking designed for professional services.

## Description
Connect your **Productive.io** account to any AI agent and take full control of your agency orchestration and project profitability through natural conversation. Productive is the premier platform for professional services automation, and this integration allows you to retrieve project metadata, monitor task statuses, and analyze financial budgets directly from your chat interface.

### What you can do

- **Project & Workflow Orchestration** — List all managed projects and retrieve detailed metadata programmatically to ensure your team's delivery is always synchronized.
- **Task & Resource Lifecycle Management** — Access and monitor project tasks and retrieve detailed status metadata including assignees and deadlines directly from the AI interface.
- **Financial & Budget Intelligence** — Access project budgets and monitor sales deals via natural language to maintain a clear overview of organizational profitability.
- **CRM & Client Control** — List companies and search through your client database to stay informed about partner relationships using simple AI commands.
- **Operational Monitoring** — Track time logs, retrieve financial invoices, and manage organization metadata to ensure your agency is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Productive.io API Token and Organization ID from your settings
3. Start managing your agency operations from Claude, Cursor, or any MCP-compatible client

No more jumping between project boards and financial reports. Your AI acts as a dedicated agency operations manager or project lead.

### Who is this for?

- **Agency Owners & Executives** — quickly retrieve profitability summaries and monitor project health without switching apps.
- **Project Managers** — automate the retrieval of task statuses and track team capacity via natural conversation.
- **Operations Teams** — streamline the retrieval of time logs and monitor financial billing directly within the chat.


## Available Tools
- **create_task**: Add new task
- **get_api_status**: Check connection
- **get_org_settings**: Get organization info
- **get_project_details**: Get project info
- **list_project_budgets**: List active budgets
- **list_client_companies**: List organizations
- **list_sales_deals**: List open deals
- **list_agency_invoices**: List financial invoices
- **list_agency_people**: List team members
- **list_agency_projects**: List all projects
- **list_project_tasks**: List tasks
- **list_time_entries**: List work logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Productive.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Productive.io."

**🤖 AI Agent:**
> I've retrieved your projects. You have 4 active environments including 'Website Redesign' and 'Mobile App Launch'. Which one would you like to see the task list for?

---

**👤 You:**
> "Show me the profitability analysis for all active projects with budget vs actual comparison."

**🤖 AI Agent:**
> 14 active projects analyzed. Total budget: $892,000. Actual spend: $634,200 (71.1% burned). 3 projects are over budget: "Website Redesign" at 112% ($56K/$50K), "Mobile App v2" at 108% ($86.4K/$80K), "Data Migration" at 104% ($52K/$50K). Most profitable: "Brand Strategy" at 62% margin ($38K cost on $100K contract). Team utilization across projects: 84%. Forecast: 2 projects will likely exceed budget by month-end based on current burn rate.

---

**👤 You:**
> "Log 6 hours of design work on the Brand Strategy project for today."

**🤖 AI Agent:**
> Time entry logged successfully. Project: Brand Strategy. Service: Design. Duration: 6 hours. Date: May 13, 2025. Billable: Yes (rate: $150/hr). Revenue generated: $900. This brings your weekly total to 28 hours across 4 projects. The Brand Strategy project has 34 of 120 budgeted hours remaining (28.3%). You are on track to complete within budget at the current pace.


## Installation & Usage

To install and use the **Productive.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/productiveio](https://vinkius.com/mcp/productiveio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
