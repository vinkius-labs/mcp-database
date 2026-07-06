# DottedSign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dottedsign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

E-signature and document management with DottedSign.

## Description
The DottedSign MCP server empowers your AI agent to manage electronic signatures, retrieve document templates, and orchestrate signing tasks entirely from the conversational interface.


## Available Tools (12)
- **create_task**: Create a new signing task
- **delete_task**: Delete a signing task
- **get_audit_trail**: Get the audit trail for a specific task
- **get_me**: Get information about the current user/token
- **list_tasks**: List all signing tasks
- **list_templates**: List all available templates
- **list_users**: List all users in the account
- **list_webhooks**: List all configured webhooks
- **retrieve_task**: Get details of a specific signing task
- **update_task**: Update an existing signing task
- **cancel_task**: Cancel an active signing task
- **create_task_from_template**: Create a new signing task from a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DottedSign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active document templates in DottedSign."

**🤖 AI Agent:**
> Retrieving your templates... You have 4 templates available. The most used one is 'Standard NDA'.

---

**👤 You:**
> "Check the status of signing task 'TASK_ID'."

**🤖 AI Agent:**
> Task 'TASK_ID' is currently 'Pending'. Only 1 out of 2 participants has signed.

---

**👤 You:**
> "Delete draft document 'DOC_ID'."

**🤖 AI Agent:**
> Draft document 'DOC_ID' has been successfully deleted from your workspace.


## ❓ FAQ

**Q: Can I automate the sending of a specific document template?**
Yes! You can use the agent to map the document template and instantly send the signing request.

**Q: How can I track the signing status of a document?**
Simply query the Task ID through the agent to retrieve its real-time signature status, whether pending or completed.

**Q: Do I need a paid plan to use the DottedSign API?**
Access to the API generally requires an active DottedSign API subscription plan. Check the official docs for current restrictions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dottedsign](https://vinkius.com/mcp/dottedsign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DottedSign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dottedsign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DottedSign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dottedsign": {
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
