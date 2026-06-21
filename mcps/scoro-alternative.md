# Scoro MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scoro-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/scoro-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/scoro-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate business management via Scoro — manage projects, sales, and billing directly with AI.

## Description
Connect your **Scoro** account to any AI agent and take full control of your business orchestration and project management through natural conversation. Scoro provides a comprehensive platform for managing your entire workspace, from CRM and sales to projects and billing, and this integration allows you to retrieve task metadata, monitor sales pipelines, and manage financial documents directly from your chat interface.

### What you can do

- **Project & Task Orchestration** — List all managed projects and retrieve detailed metadata, including task assignments and completion statuses programmatically.
- **Sales & CRM Intelligence** — Access and monitor your sales pipeline, retrieve contact metadata, and view quotes directly from the AI interface.
- **Financial & Billing Control** — Manage invoices and bills to maintain a clear overview of your business finances via natural language.
- **Account Performance Monitoring** — Retrieve real-time account metrics and monitor workspace health to ensure your operations are always optimized.
- **Operational Oversight** — Access detailed task and project metadata using simple AI commands to streamline your work management.

### How it works

1. Subscribe to this server
2. Enter your Scoro API Key and Subdomain from your account settings
3. Start managing your workspace from Claude, Cursor, or any MCP-compatible client

No more jumping between project boards and CRM lists. Your AI acts as a dedicated operations manager or project coordinator.

### Who is this for?

- **Project Managers** — quickly retrieve project statuses and monitor task deadlines without switching apps.
- **Sales Teams** — automate the retrieval of quote details and track pipeline velocity via natural conversation.
- **Finance Operations** — streamline the monitoring of invoices and bills directly within the chat.


## Available Tools
- **get_bill**: Get details for a Scoro bill
- **get_contact**: Get details for a Scoro contact
- **get_invoice**: Get details for a Scoro invoice
- **get_project**: Get details for a Scoro project
- **get_quote**: Get details for a Scoro quote
- **get_task**: Get details for a Scoro task
- **list_bills**: List supplier bills/payables
- **list_contacts**: List Scoro contacts
- **list_invoices**: List sales invoices
- **list_projects**: List all Scoro projects
- **list_quotes**: List sales quotes/proposals
- **list_tasks**: List all Scoro tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scoro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Scoro."

**🤖 AI Agent:**
> I've retrieved your projects. You have 4 active ones including 'Website Redesign' and 'Q1 Marketing Campaign'. Would you like to see the task breakdown for any of them?

---

**👤 You:**
> "Show me the profitability dashboard for all active projects with budget burn rates."

**🤖 AI Agent:**
> 12 active projects analyzed. Total revenue: $890,000. Total costs: $623,000. Overall margin: 30%. Top margin: "Brand Strategy" at 48% ($120K revenue, $62K cost). At-risk: "Mobile App v2" at 8% margin (budget 92% burned with 60% completion). "Data Migration" negative margin -5% (scope creep). Team utilization: 84% billable. Overdue invoices on projects: $45,000. Forecast: Q2 project revenue on track at $1.2M if current pipeline converts.

---

**👤 You:**
> "List all pending quotes and proposals with their expected close dates and values."

**🤖 AI Agent:**
> 18 pending quotes/proposals totaling $1.4M. Due to close this week (4): Meridian Corp $180K (90% probability), TechVentures $95K (75%), DataFlow $67K (60%), ScaleUp $45K (80%). Due within 30 days (8): $620K combined. Overdue for follow-up (6): $392K (oldest: 21 days). Win rate on similar proposals: 42%. Average time to decision: 14 days. 3 proposals need revision based on client feedback. Top contributor: James Park with $450K in active proposals.


## Installation & Usage

To install and use the **Scoro** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scoro-alternative](https://vinkius.com/mcp/scoro-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
