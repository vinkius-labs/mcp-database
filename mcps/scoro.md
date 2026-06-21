# Scoro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scoro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Bring your Scoro end-to-end work management platform into your AI workflows — query projects, invoices, and time logs seamlessly.

## Description
Connect your **Scoro** workspace to any AI agent to interact with your business operations securely. Avoid context-switching between your agency's CRM, PM software, and billing dashboards.

### What you can do

- **Project & Task Tracking** — Query your entire project portfolio, check on ongoing task statuses, and extract time entries logged by the team
- **CRM & Contacts** — Retrieve details, metadata, and history for any client or vendor in your database
- **Financial Health** — List sales invoices, pending quotes, and registered business expenses to track profitability without running manual reports
- **Team Management** — Consult your user roster, pull recent activity audit logs, and browse team calendar events directly within your chat environment

### How it works

1. Subscribe to this server
2. Enter your Scoro company subdomain and your Scoro API Key
3. Start managing your agency operations natively from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Project Managers** — instantly ask the AI to summarize all overdue tasks or compile a list of logged hours for a specific project
- **Sales & Account Executives** — pull up pending quotes and contact details before a client meeting using natural language
- **Agency Founders** — get a bird's-eye view of recent unbilled invoices or total registered expenses without navigating the full software suite


## Available Tools
- **get_contact**: Retrieves details for a specific contact
- **list_activities**: Lists recent activities and audit logs
- **list_calendar_events**: Lists all events on the Scoro calendar
- **list_contacts**: Lists all contacts (companies and people) in Scoro
- **list_expenses**: Lists all business expenses
- **list_invoices**: Lists all sales invoices
- **list_products**: Lists all products and services in the catalog
- **list_projects**: Lists all projects in Scoro
- **list_quotes**: Lists all sales quotes
- **list_tasks**: Lists all tasks
- **list_time_entries**: Lists time entries logged by the team
- **list_users**: Lists all users in the Scoro organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scoro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most recent activities logged in my Scoro workspace?"

**🤖 AI Agent:**
> Based on the recent activity logs: 1) John Doe updated the status of Task 'UI Mockups' to completed. 2) Jane Fox generated a new Quote for 'TechCorp'. 3) A new Expense was logged by Paul for $140.

---

**👤 You:**
> "List all active marketing projects and their statuses."

**🤖 AI Agent:**
> I've pulled your project portfolio. Currently, there are 3 active marketing projects: 'Q4 Global Launch' (Status: In Progress), 'SEO Overhaul 2024' (Status: Planning phase), and 'Social Media Retainer' (Status: Active). Need me to list tasks for any of these?

---

**👤 You:**
> "Show me our total revenue from the latest invoices."

**🤖 AI Agent:**
> I checked the recent sales invoices. There are 5 recent invoices generated totaling $15,400. Three of them ($8,000 total) are marked as 'paid', while two ($7,400) are 'awaiting payment'. I can format these into a markdown table if needed.


## ❓ FAQ

**Q: Can the agent calculate how many hours were logged on a specific project?**
Yes. If you ask your agent 'How many hours were logged for project Alpha recently?', the agent will invoke `list_time_entries` and filter the returned data by that specific project, summing up the billable minutes natively.

**Q: Is it possible to track unpaid invoices directly from the chat?**
Absolutely. Just prompt the AI: 'List my recent sales invoices and flag any that haven't been paid'. The agent will make an API call to `list_invoices` and analyze the 'payment status' attributes for you.

**Q: Can I retrieve contact information before a meeting?**
Yes. You can use the agent to prepare yourself. Prompt: 'Search our contacts for Acme Corp and get me their full profile'. The agent relies on `list_contacts` and `get_contact` to pull in emails, phone numbers, and relational tags.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scoro](https://vinkius.com/mcp/scoro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scoro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `scoro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scoro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scoro": {
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
