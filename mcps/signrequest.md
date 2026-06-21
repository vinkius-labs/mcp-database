# SignRequest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/signrequest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage e-signatures and documents via SignRequest — create signing requests, track document status, and manage templates directly from any AI agent.

## Description
Connect your **SignRequest** account to any AI agent to automate your document signing workflows through natural conversation.

### What you can do

- **Document Management** — List all documents, retrieve specific document details by UUID, or permanently delete documents from your account.
- **Signing Process** — Initiate signing requests by providing document URLs or templates, and track the progress of signers in real-time.
- **Template Automation** — Access and utilize reusable document templates to streamline repetitive signing tasks.
- **Webhook Integration** — Register and manage webhooks to receive instant notifications for events like document signing or declining.
- **Team & User Insights** — Retrieve information about your teams and users to manage permissions and organizational structure.

### How it works

1. Subscribe to this server
2. Enter your SignRequest API Key
3. Start managing your digital signatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & HR Teams** — quickly send out contracts or offer letters and track their status without leaving your workspace.
- **Sales Professionals** — automate the delivery of sales agreements and get notified immediately upon signature.
- **Operations Managers** — manage document templates and webhooks to integrate signing workflows into larger business processes.


## Available Tools
- **create_document**: You can provide a file URL or a template UUID, along with signers.

Create a new document in SignRequest
- **create_signrequest**: Initiate a signing process (SignRequest)
- **create_webhook**: Create a new webhook
- **delete_document**: Delete a document by UUID
- **get_document**: Retrieve a specific document by UUID
- **get_signrequest**: Retrieve a specific SignRequest by UUID
- **get_template**: Retrieve a specific template by UUID
- **list_documents**: List SignRequest documents
- **list_teams**: List teams
- **list_templates**: List available templates
- **list_users**: List users
- **list_webhooks**: List registered webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SignRequest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my recent SignRequest documents."

**🤖 AI Agent:**
> I've retrieved your documents. You have 3 recent documents: 'Service Agreement' (Status: Signed), 'NDA' (Status: Pending), and 'Offer Letter' (Status: Draft). Would you like details on any of these?

---

**👤 You:**
> "Create a new document using template UUID 550e8400-e29b-41d4-a716-446655440000 for signer test@example.com."

**🤖 AI Agent:**
> Document created successfully from the template. The document UUID is 771f9511-f30c-52e5-b827-557766551111. Should I proceed to send the signing request now?

---

**👤 You:**
> "Send document 771f9511-f30c-52e5-b827-557766551111 for signature with the message 'Please sign the agreement'."

**🤖 AI Agent:**
> The signing request has been sent for document 771f9511-f30c-52e5-b827-557766551111. I've included your custom message. You can track its status using the `get_signrequest` tool.


## ❓ FAQ

**Q: Can I check the current status and signers of a specific document?**
Yes! Use the `get_document` tool with the document's UUID. The agent will return the document's status, signer details, and other metadata.

**Q: How do I see which reusable templates are available in my account?**
Simply ask the agent to run the `list_templates` action. It will provide a list of all configured templates that you can use to create new documents.

**Q: Is it possible to automate notifications when a document is signed?**
Yes, you can use the `create_webhook` tool to register a URL that will receive real-time notifications for events like `document_signed` or `signer_signed`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signrequest](https://vinkius.com/mcp/signrequest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SignRequest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `signrequest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SignRequest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "signrequest": {
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
