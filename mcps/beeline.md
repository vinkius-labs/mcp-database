# Beeline MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beeline)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/beeline-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/beeline-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage your external workforce via Beeline VMS — list assignments, requisitions, and timesheets directly from any AI agent.

## Description
Connect your **Beeline Vendor Management System (VMS)** account to any AI agent and orchestrate your contingent workforce operations through natural conversation.

### What you can do

- **Assignment Oversight** — List and inspect active work assignments to monitor external talent deployment.
- **Requisition Management** — Query job requisitions and search for open postings within your organization.
- **Time & Expense Tracking** — Retrieve submitted timesheets and expense reports for auditing and approval workflows.
- **Supplier Management** — List and verify the vendors and suppliers linked to your Beeline account.
- **User Auditing** — Retrieve account profile information to ensure correct system access.

### How it works

1. Subscribe to this server
2. Enter your Beeline OAuth Access Token
3. Start managing your external talent from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Hiring Managers** — instantly check the status of job requisitions without logging into the VMS dashboard.
- **Procurement Teams** — audit supplier lists and assignment metadata straight from their workflow tools.
- **HR Ops** — retrieve timesheet summaries and assignment details during workforce planning meetings.


## Available Tools
- **get_assignment**: Get details of a specific assignment
- **get_requisition**: Get details of a job requisition
- **get_timesheet**: Get details of a specific timesheet
- **get_user_info**: Get Beeline user profile
- **list_assignments**: List active work assignments
- **list_expenses**: List expense reports
- **list_requisitions**: List job requisitions
- **list_suppliers**: List vendors/suppliers
- **list_timesheets**: List submitted timesheets
- **search_requisitions**: Search job requisitions by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active assignments in Beeline."

**🤖 AI Agent:**
> I've retrieved 5 active assignments. Key entries include 'Senior Developer - Q2' (ID: asgn_123) and 'Project Manager - Retail' (ID: asgn_456). Which one would you like more details on?

---

**👤 You:**
> "Search for open requisitions matching 'React'."

**🤖 AI Agent:**
> I found 2 open requisitions matching 'React': 'Frontend Engineer (Mid-level)' (ID: req_992) and 'Fullstack JS Developer' (ID: req_995). Would you like to see the full requirements for either?

---

**👤 You:**
> "Show me recent timesheets that need review."

**🤖 AI Agent:**
> Retrieving recent timesheets... I found 8 entries from last week. All have been submitted by contractors and are awaiting manager review in the Beeline dashboard.


## Installation & Usage

To install and use the **Beeline** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beeline](https://vinkius.com/mcp/beeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
