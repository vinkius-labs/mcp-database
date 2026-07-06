# SuiteDash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/suitedash)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage CRM, projects, tasks, and invoices on SuiteDash with AI agents.

## Description
Connect your **SuiteDash** account to any AI agent to automate your client portal and business management. SuiteDash provides a comprehensive all-in-one platform for CRM, project management, and billing, and this integration allows you to retrieve contact metadata, monitor project progress, and track invoices through natural conversation.

### What you can do

- **CRM & Contact Orchestration** — List and search through your contact and company database, including creating new records programmatically.
- **Project & Task Lifecycle Management** — List all managed projects and tasks to ensure your team's workflow is always synchronized directly from the AI interface.
- **Billing & Financial Monitoring** — Access and monitor invoices, estimates, and deals to maintain a clear overview of your business revenue.
- **Custom Schema Intelligence** — Retrieve contact metadata schemas to ensure your data entry is always consistent with your account's custom fields.
- **Operational Oversight** — Track project health and manage business relationships via natural language commands.

### How it works

1. Subscribe to this server
2. Enter your SuiteDash Public ID and Secret Key from your Secure API settings
3. Start managing your business portal from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agency Owners** — quickly retrieve client details and monitor project statuses without switching apps.
- **Project Managers** — automate the retrieval of task lists and monitor team assignments via natural conversation.
- **Operations Teams** — streamline the management of invoices and monitor deal progress directly within the chat.


## Available Tools (11)
- **get_contact_details**: Get details for a contact
- **get_schema_metadata**: Get CRM field definitions
- **get_project_details**: Get metadata for a project
- **list_companies**: List CRM companies
- **list_contacts**: List CRM contacts
- **list_deals**: List sales deals
- **list_invoices**: List invoices
- **list_projects**: List active projects
- **list_tasks**: List project tasks
- **create_contact**: Register a new contact
- **get_company_details**: Get details for a company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SuiteDash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in SuiteDash."

**🤖 AI Agent:**
> I've retrieved your projects. You have 4 active environments including 'Website Redesign', 'Marketing Strategy 2024', and 'New Product Launch'. Which one would you like to see tasks for?

---

**👤 You:**
> "Show me all active client projects with their task progress and billing status."

**🤖 AI Agent:**
> 12 active client projects. By status: On Track (7): avg 65% complete. "Meridian Corp Rebrand" (82%, billing current, $45K invoiced of $60K). "TechVentures App" (71%, $23K of $35K). At Risk (3): "DataFlow Migration" (34%, 2 weeks behind, resource gap). Overdue (2): "ScaleUp Website" (90% complete, final review pending). Total billable hours this month: 890. Unbilled time: 45 hours ($6,750). Client portal logins this week: 34. File shares: 123 documents across all projects.

---

**👤 You:**
> "Create a new client workspace for Meridian Corp with CRM, project, and billing modules enabled."

**🤖 AI Agent:**
> Client workspace created: Meridian Corp. Modules enabled: CRM (contacts, pipeline), Projects (tasks, Gantt, Kanban), Billing (invoices, estimates, payments). Portal URL: app.yourdomain.com/meridian-corp. Admin users: 2 (David Chen CEO, Sarah Williams PM). Client portal access: enabled with branded login page. File storage: 10 GB allocated. Integration: Stripe connected for online payments. Automation: welcome email sent, onboarding checklist created (8 tasks). Template applied: "Enterprise Client" workflow.


## ❓ FAQ

**Q: How do I find my SuiteDash API credentials?**
Log in to your SuiteDash portal, navigate to **Integrations** > **Secure API**, and you will find your unique **Public ID** and **Secret Key** there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/suitedash](https://vinkius.com/mcp/suitedash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SuiteDash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `suitedash` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SuiteDash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "suitedash": {
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
