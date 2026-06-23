# Avaza MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/avaza)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Unified project management, time tracking, and invoicing via Avaza — orchestrate professional services natively via AI.

## Description
Connect your **Avaza** account to any AI agent and manage your entire professional services lifecycle through natural conversation.

### What you can do

- **Project & Task Operations** — Create, update, and list projects and tasks to keep your team aligned and on schedule
- **Smart Time Tracking** — Log and audit timesheet entries for accurate resource management and billing
- **CRM & Financial Insights** — Access company contacts and retrieve recent invoices for full visibility into project financials
- **Resource Coordination** — Programmatically manage your professional services workflows and team allocations

### How it works

1. Subscribe to this server
2. Enter your Avaza Personal Access Token
3. Start managing your professional services from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — instantly retrieve project statuses, list stale tasks, and audit billable hours
- **Agencies & Consultants** — log time and manage client invoices directly from your workspace to avoid context switching
- **Team Leads** — coordinate task assignments and check team availability through natural language commands


## Available Tools (11)
- **create_project**: Create a new project
- **create_task**: Create a new task in a project
- **create_timesheet**: Create a new timesheet entry
- **get_account_check**: Verify Avaza account connection
- **get_project**: Get details for a specific project
- **list_contacts**: List company contacts and users
- **list_invoices**: List recent invoices
- **list_projects**: List all Avaza projects
- **list_tasks**: List all Avaza tasks
- **list_timesheets**: List timesheet entries
- **update_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Avaza** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Avaza."

**🤖 AI Agent:**
> I've retrieved your projects. You have 3 active environments: 'Website Redesign', 'Q4 Marketing Strategy', and 'Client Onboarding'. Which one would you like to drill into for task details?

---

**👤 You:**
> "Create a new task 'Prepare Financial Audit' in project ID 12345."

**🤖 AI Agent:**
> The task 'Prepare Financial Audit' has been successfully created in project 12345. I've assigned a high priority to it based on your request. Would you like me to set a deadline?

---

**👤 You:**
> "Log 2 hours of work for today on project 'Website Redesign'."

**🤖 AI Agent:**
> Timesheet entry created! I've logged 2 hours for today on 'Website Redesign' (Project ID: 54321). Your total logged hours for this project are now updated.


## ❓ FAQ

**Q: Can the AI automatically log time for a specific project?**
Yes! Use the `create_timesheet` tool. You'll need to provide the ProjectID, PersonID, and the duration to instantly log work hours in your Avaza account.

**Q: How do I update the status of a task through the AI?**
Simply ask the agent to run the `update_task` tool with the TaskID. You can modify the title, description, or status to reflect the current progress of your work.

**Q: Does this integration allow for auditing recent customer invoices?**
Yes. The `list_invoices` tool provides a clear overview of recent billing, helping you track payment statuses and financial health across your projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avaza](https://vinkius.com/mcp/avaza)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Avaza** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `avaza` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Avaza** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "avaza": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
