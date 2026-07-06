# Yida MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yida)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enterprise low-code development platform by DingTalk — manage forms, data instances, and approval workflows via AI.

## Description
Empower your AI agent to orchestrate your enterprise operations with **Yida**, the premier low-code platform under the DingTalk ecosystem. By connecting Yida to your agent, you transform complex form management and data orchestration into a natural conversation. Your agent can instantly list your forms, retrieve field schemas, manage data records (create, update, delete), and even monitor workflow approval timelines without you needing to navigate the complex DingTalk interface. Whether you are managing administrative approvals, inventory tracking, or customized business processes, your agent acts as a real-time operations assistant, keeping your data accurate and your workflows moving.

### What you can do

- **Form Orchestration** — List all accessible forms and retrieve detailed field schemas for your Yida applications.
- **Data Operations** — Manage form instances (records) with full support for creating, listing, and granular updates.
- **Workflow Monitoring** — Check the current status and approval timeline for any workflow instance.
- **Schema Auditing** — Retrieve internal form schemas to understand data structures and field IDs.
- **User Coordination** — Access application user lists to manage assignments and participation effectively.

### How it works

1. Subscribe to this server
2. Enter your DingTalk App Key, App Secret, and Yida App Code
3. Start managing your enterprise applications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Enterprise Operations** — automate data entry and monitor approval workflows through natural language.
- **Department Managers** — oversee project data and internal requests through a unified AI interface.
- **IT Administrators** — monitor form schemas and automated workflows without manual technical overhead.
- **DingTalk Users** — integrate your existing Yida workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_form_schema**: Get form field schema
- **get_instance_timeline**: Get workflow instance timeline
- **get_record_details**: Get record detailed data
- **list_data_ids**: List data instance IDs
- **list_forms**: List all forms in the Yida application
- **list_users**: List application users
- **list_workflows**: List application workflows
- **update_record**: Update an existing record
- **create_record**: Create a new form record
- **delete_record**: Delete a form record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yida** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all forms in my Yida application."

**🤖 AI Agent:**
> I've retrieved the forms for your Yida application. You have 4 forms: 'Purchase Request', 'Inventory Audit', 'Employee Onboarding', and 'Travel Expense'. Which one would you like to view data for?

---

**👤 You:**
> "Show me the last 5 instance IDs from the 'Purchase Request' form."

**🤖 AI Agent:**
> I've listed the last 5 instance IDs for 'Purchase Request'. They include REQ-2026-001 through REQ-2026-005. Would you like to see the detailed field data for any of these requests?

---

**👤 You:**
> "What is the approval timeline for purchase request 'REQ-2026-042'?"

**🤖 AI Agent:**
> The purchase request 'REQ-2026-042' is currently pending with the Finance Director. It was approved by the Department Head at 10 AM today. Should I send a follow-up notification?


## ❓ FAQ

**Q: How do I find my DingTalk App Key and Secret?**
Log in to the DingTalk Developer Backend, create or select an 'Internal Enterprise Application', and you will find the App Key and App Secret under the 'Credentials' section.

**Q: Where can I find the Yida 'App Code'?**
Open your Yida application, go to [Settings] → [Deployment and O&M], and you will find the 'App Code' (Application Code) there. It is required for all Yida API calls.

**Q: Can I see the approval history of a record?**
Yes. Use the `get_instance_timeline` tool with the form instance ID. It will return the full approval history, including who approved it and at what time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yida](https://vinkius.com/mcp/yida)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yida** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yida` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yida** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yida": {
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
