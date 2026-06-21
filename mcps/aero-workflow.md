# Aero Workflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aero-workflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize accounting firm tasks, track client work, and manage team workloads with purpose-built practice management.

## Description
Connect your **Aero Workflow** account to any AI agent and take full control of your accounting practice management and automated firm operations through natural conversation.

### What you can do

- **Workflow & Task Orchestration** — List and manage your entire practice hierarchy programmatically, retrieving detailed checklists and high-fidelity technical instructions in real-time
- **Time Tracking Intelligence** — Monitor billable hour records and retrieve detailed historical time logs to maintain a perfectly coordinated overview of staff productivity
- **Customer Lifecycle Management** — Access complete directories of firm customers and business entities to coordinate your organizational relationship ecosystem programmatically
- **Communication Architecture** — Access and monitor workflow-linked emails and message threads to maintain high-fidelity oversight of client interactions
- **Infrastructure Monitoring** — Retrieve checklist templates and verify account-level settings directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Account ID** (from your URL) and **API Key** from your Aero Workflow admin settings
3. Start orchestrating your firm's productivity from Claude, Cursor, or any MCP client

No more manual status checking of individual tasks or digging through complex time sheets. Your AI acts as your dedicated practice coordinator and operations analyst.

### Who is this for?

- **Accountants & Bookkeepers** — instantly retrieve task summaries and log billable hours using natural language commands
- **Firm Owners & Managers** — monitor staff capacity and track client workflow health without leaving your workspace
- **Operations Leads** — automate the management of reusable checklist templates through simple AI queries


## Available Tools
- **check_api_health**: Verify Aero Workflow API status
- **create_new_customer**: Requires name and contact information.

Add a new client to Aero
- **create_new_workflow_task**: Requires a subject and assigned user.

Add a new task to Aero
- **get_account_info**: Get account metadata
- **get_task_details**: Get details for a specific task
- **list_firm_customers**: List all client accounts
- **list_workflow_emails**: List communication emails
- **list_workflow_tasks**: List workflow tasks and checklists
- **list_checklist_templates**: List reusable workflow templates
- **list_time_tracking_logs**: List time entries for tasks
- **list_firm_team_members**: List firm users and staff
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aero Workflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workflow tasks in my Aero account."

**🤖 AI Agent:**
> I've retrieved your active tasks. You currently have 5 workflows in progress, including 'Monthly Reconciliation' and 'Payroll Audit'. Would you like the detailed high-fidelity checklists for any of these?

---

**👤 You:**
> "Create a new task 'Urgent Tax Review' for customer 'Acme Corp'."

**🤖 AI Agent:**
> Workflow task created! I've successfully registered 'Urgent Tax Review' for Acme Corp. It's now visible to your staff in the Aero dashboard. Shall I list your available checklist templates to attach instructions?

---

**👤 You:**
> "Show my recent time tracking logs for this week."

**🤖 AI Agent:**
> Accessing productivity data... For this week, your firm has logged a total of 120 billable hours across 8 active clients. Highlights include 40 hours for 'Global Tech'. Need the high-fidelity staff utilization report?


## ❓ FAQ

**Q: How do I find my Aero Account ID and API Key?**
Log in as an Admin, navigate to **Admin** > **Aero API** to generate your key. Your Account ID is the unique identifier in your browser's URL.

**Q: Can I record time logs via AI?**
Yes! The `create_new_workflow_task` tool allows you to include time metadata when creating or updating tasks to maintain accurate high-fidelity billing records.

**Q: How do I retrieve client directories?**
Use the `list_firm_customers` tool to retrieve your complete directory of managed business entities and individual client accounts programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aero-workflow](https://vinkius.com/mcp/aero-workflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aero Workflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `aero-workflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aero Workflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aero-workflow": {
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
