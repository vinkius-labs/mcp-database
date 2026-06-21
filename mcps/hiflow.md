# HiFlow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hiflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Workflow and business process management.

## Description
The HiFlow MCP server bridges your AI agent with your enterprise workflows. Trigger processes, approve pending steps, and query real-time process states through a seamless conversational interface.


## Available Tools
- **create_customer**: Create a new customer
- **get_activity**: Retrieve activity dashboard information
- **get_customer**: Retrieve details for a specific customer
- **get_estimate**: Retrieve details for a specific estimate
- **get_invoice**: Retrieve details for a specific invoice
- **get_job**: Retrieve details for a specific job
- **get_me**: Retrieve information about the current user
- **list_customers**: List all customers
- **list_estimates**: List all estimates (quotes)
- **list_invoices**: List all invoices
- **list_jobs**: List all jobs/projects
- **list_timesheets**: List all timesheet entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HiFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my pending approvals."

**🤖 AI Agent:**
> You have 3 pending approvals in the queue. The most urgent is 'Invoice #1042 Approval' assigned 2 days ago.

---

**👤 You:**
> "Start the 'Employee Onboarding' process for John Doe."

**🤖 AI Agent:**
> The 'Employee Onboarding' process has been started (Instance ID: 5041).

---

**👤 You:**
> "Approve task ID 9481."

**🤖 AI Agent:**
> Task 9481 has been marked as 'Approved' and the workflow has advanced to the next stage.


## ❓ FAQ

**Q: Can I start a new workflow from the AI?**
Yes, you can trigger new workflow instances by specifying the process ID and required variables.

**Q: How do I check pending tasks?**
Ask the agent to 'List my pending approvals', and it will retrieve the queue of tasks requiring your attention.

**Q: Is it possible to approve a task directly in the chat?**
Yes! Provide the task ID and tell the agent to mark it as approved or rejected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hiflow](https://vinkius.com/mcp/hiflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HiFlow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hiflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HiFlow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hiflow": {
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
