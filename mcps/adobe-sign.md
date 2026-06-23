# Adobe Sign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adobe-sign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Automate e-signatures and document workflows via Adobe Acrobat Sign — manage agreements, track audit trails, and handle library templates directly from your AI agent.

## Description
Connect **Adobe Acrobat Sign** to your AI agent to streamline your digital signature workflows and document management through natural language.

### What you can do

- **Agreement Management** — List all active agreements, create new ones, and fetch detailed metadata for specific contracts.
- **Document Retrieval** — Download combined PDF documents or specific audit trails to verify the legality and history of any signature process.
- **Library & Templates** — Access and manage your organization's library documents and templates to reuse standard forms efficiently.
- **Transient Documents** — Upload temporary files to the Adobe Sign cloud to be used in immediate agreement creation workflows.
- **Admin & Webhooks** — Monitor real-time events via webhooks and manage users or groups within your Adobe Sign account.

### How it works

1. Subscribe to this server
2. Provide your Adobe Sign Access Token and API URL
3. Start managing your legal workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & Compliance Teams** — quickly verify the status of pending contracts and retrieve audit trails without manual searching.
- **Sales Operations** — automate the creation of agreements and track which clients have signed in real-time.
- **HR Departments** — manage employee onboarding documents and library templates directly through an AI assistant.


## Available Tools (13)
- **create_agreement**: Create a new agreement
- **create_library_document**: Create a library document
- **create_transient_document**: g., creating an agreement). Available for 7 days.

Upload a transient document
- **create_user**: Create a new user
- **create_webhook**: Create a new webhook
- **get_agreement**: Get agreement metadata
- **get_agreement_audit_trail**: Download the audit trail PDF for an agreement
- **get_agreement_combined_document**: Download all documents in a single PDF
- **list_agreements**: List agreements
- **list_groups**: List groups in the account
- **list_library_documents**: List library documents
- **list_users**: List users in the account
- **list_webhooks**: List webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adobe Sign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current agreements in Adobe Sign."

**🤖 AI Agent:**
> I've retrieved your agreements. You have 3 active agreements: 'Service Contract - Q4', 'NDA - New Hire', and 'Vendor Agreement'. Would you like to see the details for any of these?

---

**👤 You:**
> "Get the metadata for agreement ID 3AAABLblqZhD123."

**🤖 AI Agent:**
> The agreement 'Service Contract - Q4' (ID: 3AAABLblqZhD123) is currently in 'OUT_FOR_SIGNATURE' status. It was created on Oct 12th and is waiting for a signature from client@example.com.

---

**👤 You:**
> "Show me all users registered in our Adobe Sign account."

**🤖 AI Agent:**
> I found 5 users in your account, including 'Admin User', 'Legal Lead', and 3 staff members. Would you like to see the specific group assignments for these users?


## ❓ FAQ

**Q: How can I verify the legal history of a signed document?**
You can use the `get_agreement_audit_trail` tool with the specific Agreement ID. The agent will retrieve the official audit trail PDF containing all timestamps and participant actions.

**Q: Can I see a list of all templates available in my organization?**
Yes! By running the `list_library_documents` tool, your AI agent will display all stored templates and library documents you have access to.

**Q: What is a transient document and how do I use it?**
A transient document is a temporary file upload (valid for 7 days). Use the `create_transient_document` tool to upload a file, which then provides an ID you can use to create a formal agreement via `create_agreement`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adobe-sign](https://vinkius.com/mcp/adobe-sign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adobe Sign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adobe-sign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adobe Sign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adobe-sign": {
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
