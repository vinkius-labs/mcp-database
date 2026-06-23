# Simplicate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplicate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Dutch professional services firm with CRM, project management, and invoicing designed for the Benelux market.

## Description
Connect your **Simplicate** account to any AI agent and take full control of your business workflow and project orchestration through natural conversation. Simplicate provides a comprehensive platform for CRM, sales tracking, and project management, and this integration allows you to retrieve organization metadata, monitor sales pipelines, and log hours directly from your chat interface.

### What you can do

- **CRM & Contact Orchestration** — List all managed organizations and persons to maintain a clear overview of your professional relationships programmatically.
- **Sales & Pipeline Management** — Access and monitor your sales opportunities and retrieve detailed metadata to ensure your funnel is always synchronized directly from the AI interface.
- **Project Lifecycle Control** — List and monitor active projects and services to track progress and team assignments via natural language.
- **Time Tracking Automation** — Log work hours and retrieve time-related metadata using simple AI commands to streamline your administrative tasks.
- **Operational Monitoring** — Access HRM data, monitor invoices, and retrieve organizational profile metadata to ensure your business stack is fully integrated.

### How it works

1. Subscribe to this server
2. Enter your Simplicate Domain Prefix, API Key, and API Secret from your settings
3. Start managing your business workflows from Claude, Cursor, or any MCP-compatible client

No more manual status checking or spreadsheet time logging. Your AI acts as a dedicated operations manager or project coordinator.

### Who is this for?

- **Agency Owners** — quickly retrieve client details and monitor project profitability without switching apps.
- **Sales Managers** — automate the retrieval of deal statuses and monitor pipeline metrics via natural conversation.
- **Operations Teams** — streamline the logging of hours and monitor organizational health directly within the chat.


## Available Tools (12)
- **get_my_organization_profile**: Get authenticated organization profile
- **get_project_details**: Get details for a specific project
- **get_sales_details**: Get details for a specific sales opportunity
- **list_employees**: List all company employees
- **list_time_registrations**: List time entries
- **list_invoices**: List all invoices
- **list_crm_organizations**: List all organizations/companies
- **list_crm_persons**: List all individual contacts
- **list_projects**: List all projects
- **list_sales_opportunities**: List all sales opportunities
- **list_project_services**: List available project services
- **log_time_registration**: Register new hours worked


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simplicate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in Simplicate."

**🤖 AI Agent:**
> I've retrieved your projects. You have 5 active environments including 'IT Infrastructure Audit', 'Marketing Campaign Q1', and 'HR System Implementation'. Which one would you like to log hours for?

---

**👤 You:**
> "Log 2 hours for project ID 'proj-123' with description 'Code review'."

**🤖 AI Agent:**
> Work log registered! I've successfully added 2 hours to project 'proj-123'. Would you like me to check your total logged hours for this week?

---

**👤 You:**
> "Show me the pipeline for my active sales opportunities."

**🤖 AI Agent:**
> Fetching sales pipeline... You have 3 opportunities in 'Quotation' stage and 1 in 'Negotiation'. Would you like the full details for the 'Cloud Migration' deal?


## ❓ FAQ

**Q: Can my AI automatically log hours for a specific project just by providing the project ID and duration?**
Yes! Use the `log_hours` tool. Provide the Project ID, start time, end time, and a description, and your agent will register the work log in Simplicate instantly.

**Q: How do I check the current status of a sales opportunity?**
Simply ask the agent to run the `get_sales_details` action with the Sale ID. It will retrieve the detailed metadata, including the current stage in your pipeline.

**Q: How do I find my Simplicate API credentials and Domain Prefix?**
Log in to your Simplicate account, navigate to **Settings** > **General** > **API**, and you will find your Authentication Key and Secret. Your Domain Prefix is the first part of your Simplicate URL (e.g., 'prefix'.simplicate.nl).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplicate](https://vinkius.com/mcp/simplicate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Simplicate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simplicate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Simplicate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simplicate": {
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
