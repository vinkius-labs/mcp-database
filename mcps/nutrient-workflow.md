# Nutrient Workflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nutrient-workflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Build document workflows with PDF viewing, editing, annotation, and digital signatures embedded directly into your applications.

## Description
Connect your **Nutrient Workflow** (formerly Integrify) environment to any AI agent and streamline your enterprise automation and task management through natural conversation.

### What you can do

- **Process Control** — List all published workflow processes and retrieve detailed configuration metadata
- **Request Management** — Start new workflow instances and track the status of active or historical requests
- **Task Execution** — Query pending tasks for any user and complete them programmatically with form data
- **System Overview** — List registered users and available reports to monitor your organizational efficiency

### How it works

1. Subscribe to this server
2. Enter your Tenant ID, Host, and API Key from your system settings
3. Start managing your enterprise workflows from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **complete_task**: Complete a workflow task
- **get_process**: Get details for a specific process
- **get_request**: Get details for a specific request
- **get_task**: Get details for a specific task
- **list_processes**: List Nutrient Workflow processes
- **list_reports**: List available reports
- **list_requests**: List active workflow requests
- **list_user_tasks**: List pending tasks for a user
- **list_users**: List tenant users
- **start_request**: Start a new workflow request


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nutrient Workflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active workflow processes."

**🤖 AI Agent:**
> I've fetched your processes. You have 5 active workflows, including 'Expense Approval', 'Onboarding', and 'IT Support Ticket'.

---

**👤 You:**
> "Find pending tasks for user 'admin_123'."

**🤖 AI Agent:**
> User 'admin_123' has 3 pending tasks: 2 Expense Approvals and 1 Budget Review. Would you like the details for the first one?

---

**👤 You:**
> "Start a new 'Expense Approval' request."

**🤖 AI Agent:**
> Request started! I've triggered a new instance of the 'Expense Approval' workflow. The new Request ID is 'req_777'.


## ❓ FAQ

**Q: Can I list all my business processes using my AI agent?**
Yes! Use the `list_processes` tool to retrieve a full list of all published workflow processes in your tenant.

**Q: How do I start a new workflow request through this integration?**
Simply provide the Process ID to the `start_request` tool. You can also pass initial form data as a JSON object.

**Q: Is it possible to complete a task via the AI agent?**
Yes, use the `complete_task` action. Provide the Task ID and any required form data to progress the workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nutrient-workflow](https://vinkius.com/mcp/nutrient-workflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nutrient Workflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nutrient-workflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nutrient Workflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nutrient-workflow": {
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
