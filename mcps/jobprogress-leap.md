# JobProgress (Leap) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jobprogress-leap)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage contractors, customers, and jobs via JobProgress API.

## Description
Empower your AI agents with JobProgress's (now part of Leap) business management platform for contractors. This MCP server allows you to list and retrieve customers and jobs, track estimates and proposals, manage workflows and tasks, and view appointments directly through the JobProgress API. Ideal for automating construction and home improvement operations.


## Available Tools (10)
- **get_customer**: Returns addresses, project history, and custom metadata. Essential for deep intelligence on a customer before preparing estimates or jobs.

Retrieves details for a specific customer
- **get_job**: Returns project descriptions, cost estimates, and current stage in the workflow. Use this to analyze a project's progress or provide customer updates.

Retrieves details for a specific job
- **list_appointments**: Essential for managing the field service calendar.

Lists all scheduled appointments
- **list_customers**: Returns customer names, contact info, and IDs. Use this as the main starting point for customer management or finding a specific client.

Lists all customers in JobProgress
- **list_estimates**: Useful for auditing sales performance and identifying pending project approvals.

Lists all job estimates
- **list_jobs**: Includes job titles, status, and associated customer IDs. Use this to monitor the project pipeline and upcoming work.

Lists all jobs in JobProgress
- **list_proposals**: Useful for monitoring contract acceptance and sales conversions.

Lists all job proposals
- **list_tasks**: Essential for helping the user manage their daily to-do list.

Lists all tasks
- **list_users**: Useful for identifying assignees or sales reps.

Lists all users in the organization
- **list_workflows**: Useful for understanding business processes.

Lists all configured workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JobProgress (Leap)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active customers in JobProgress."

**🤖 AI Agent:**
> I'll fetch the list of your active customers from JobProgress.

---

**👤 You:**
> "Show me the details for job ID '123'."

**🤖 AI Agent:**
> I'll retrieve the full details and current status for that specific job.

---

**👤 You:**
> "Check my appointments for today."

**🤖 AI Agent:**
> I'll look up your scheduled appointments in JobProgress for you.


## ❓ FAQ

**Q: How do I get JobProgress API credentials?**
Log in to your JobProgress account, navigate to Settings > Developer, and generate a new Access Token.

**Q: Are estimates and proposals supported?**
Yes, you can list and retrieve data for both estimates and proposals using the corresponding tools in this MCP.

**Q: Can I see my schedule?**
Yes, the list_appointments tool allows you to retrieve scheduled appointments from your JobProgress account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jobprogress-leap](https://vinkius.com/mcp/jobprogress-leap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JobProgress (Leap)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jobprogress-leap` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JobProgress (Leap)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jobprogress-leap": {
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
