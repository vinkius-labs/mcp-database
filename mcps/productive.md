# Productive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/productive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/productive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/productive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Manage your entire agency workflow via Productive — fetch budgets, analyze time entries, track deals, and monitor project health directly from any AI agent.

## Description
Connect your **Productive** account to any AI agent and bring your agency management data directly into your conversation workflow.

### What you can do

- **Projects & Budgets** — List all active projects, retrieve detailed project data, and dive deep into financial budgets to monitor burn rates
- **Time Tracking & Tasks** — Audit logged time entries across your team and track task progress on any board instantly
- **Sales & CRM** — List all open deals, review the sales pipeline, and access full company/client databases without switching tabs
- **Financials** — Access all generated invoices and their payment statuses to keep cash flow in check
- **People & Activity** — Track recent activities, team availability, and audit logs to see exactly what's moving in your agency

### How it works

1. Subscribe to this server
2. Enter your Productive API Token and Organization ID
3. Start managing your agency operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agency Founders & Executives** — ask your agent for a daily summary of billable hours, burning budgets, and unpaid invoices
- **Project Managers** — instantly check task progress, team capacities, and recent project activities in natural language
- **Sales Teams** — pull up client information and active deals to prepare for calls faster


## Available Tools
- **list_projects**: Ideal for scoping agency workload.

Lists all active and archived projects in Productive
- **get_project**: Retrieves details for a single project by ID
- **list_people**: Lists all people, including employees and external contacts
- **list_services**: Use this to check billable items.

Lists all services defined in the organization
- **list_deals**: Lists all sales deals and their current stages
- **list_tasks**: Lists all tasks across the organization
- **list_time_entries**: Lists time entries logged by the team
- **list_invoices**: Lists all generated invoices and their payment status
- **list_budgets**: Lists all project budgets
- **list_companies**: Lists all companies (clients and partners) in the CRM
- **list_boards**: Lists all task boards
- **list_activities**: Lists recent activities and audit logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Productive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze our active budgets and find any approaching their limit."

**🤖 AI Agent:**
> I've reviewed the budgets. You have 3 budgets showing concern: 'Website Redesign' is at 88% burn rate, and 'Q3 Marketing' is currently over budget by 4 hours. Would you like me to pull the individual time entries for those projects?

---

**👤 You:**
> "Show me unpaid invoices from last month."

**🤖 AI Agent:**
> You have 4 unpaid invoices generated last month totaling $12,500. Two of them are assigned to Acme Corp. Shall I pull up the company contact information to assist with follow-ups?

---

**👤 You:**
> "What did the development team log time on today?"

**🤖 AI Agent:**
> I checked today's time entries. The team logged a total of 26 billable hours. 14 hours went to the 'Mobile App MVP' tasks, and 12 hours were split among maintenance tickets. Overall, zero unassigned internal time was recorded.


## Installation & Usage

To install and use the **Productive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/productive](https://vinkius.com/mcp/productive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
