# QingFlow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qingflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Leading no-code BPM automation platform — manage applications, data records, and workflows via AI.

## Description
Empower your AI agent to orchestrate your business processes with **QingFlow**, the premier no-code BPM platform for digital transformation. By connecting QingFlow to your agent, you transform complex application management and data orchestration into a natural conversation. Your agent can instantly list your applications, retrieve form schemas, manage records (create, update, delete), and even monitor workflow approval statuses without you ever needing to navigate the technical dashboard. Whether you are managing procurement, HR approvals, or project tracking, your agent acts as a real-time process manager, ensuring your business logic is always executed and optimized.

### What you can do

- **Application Orchestration** — List all accessible applications and browse their internal structures.
- **Data Management** — Manage application records with full support for creating, listing, and granular updates.
- **Workflow Monitoring** — Check the current status of automated workflows and approval processes for any record.
- **Schema Auditing** — Retrieve application schemas to understand field structures and widget IDs.
- **User Coordination** — Access workspace user lists to manage assignments and participation effectively.

### How it works

1. Subscribe to this server
2. Enter your QingFlow Access Token
3. Start managing your business processes through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Leaders** — automate business processes and monitor operational KPIs through natural language.
- **Digital Transformation Officers** — oversee multiple no-code applications and workflow structures through a unified AI interface.
- **Department Managers** — manage approvals and data records directly from your AI-powered workspace.
- **IT Administrators** — monitor application schemas and automated workflows without manual technical overhead.


## Available Tools (10)
- **create_record**: Create a new application record
- **delete_record**: Delete an application record
- **get_app_schema**: Get application field schema
- **get_record_details**: Get record detailed data
- **get_workflow_status**: Get record workflow status
- **list_apps**: List all QingFlow applications
- **list_data**: List records in an application
- **list_users**: List workspace users
- **list_workflows**: List application workflows
- **update_record**: Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QingFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all applications in my QingFlow workspace."

**🤖 AI Agent:**
> I've retrieved your QingFlow applications. You have 5 active apps, including 'Expense Reimbursement', 'Leave Request', and 'Asset Management'. Which one would you like to explore?

---

**👤 You:**
> "Show me the records for the 'Asset Management' application."

**🤖 AI Agent:**
> I've listed the records for 'Asset Management'. I found 12 items, including 'MacBook Pro #001' and 'Dell Monitor #042'. Would you like the details of a specific record?

---

**👤 You:**
> "What is the approval status for record 'req-9920' in 'Leave Request'?"

**🤖 AI Agent:**
> The leave request 'req-9920' is currently at the 'Department Head Approval' stage. It has been pending for 2 hours. Would you like me to send a reminder?


## ❓ FAQ

**Q: How do I find my QingFlow Access Token?**
Log in to QingFlow, go to the Qing Store (轻商城), install the 'OPEN API' plugin under Third-party Connections, and find your Access Token in the plugin configuration.

**Q: Can I check why a request is pending approval?**
Yes. Using the `get_workflow_status` tool with the application and record IDs, you can retrieve the current approval node, the person responsible, and the status of the process.

**Q: How do I format the data for creating a record?**
QingFlow uses a specific format for its fields. Use the `get_app_schema` tool first to see the `queId` for each field, then provide the data as a JSON string following the required structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qingflow](https://vinkius.com/mcp/qingflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QingFlow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qingflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QingFlow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qingflow": {
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
