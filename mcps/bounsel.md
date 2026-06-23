# Bounsel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bounsel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your contract lifecycle via Bounsel — list documents, automate templates, and request signatures directly from any AI agent.

## Description
Connect your **Bounsel** CLM account to any AI agent and orchestrate your legal document workflows through natural conversation.

### What you can do

- **Document Oversight** — List and retrieve detailed metadata for all your generated contracts and legal documents.
- **Automated Drafting** — Create new documents instantly by merging your data with pre-configured smart templates.
- **Template Discovery** — List available templates and their required fields to ensure accurate data entry.
- **Signature Orchestration** — Initiate the digital signature process for any completed document.
- **Document Lifecycle** — Delete drafts or canceled documents to maintain a clean workspace.
- **Team Management** — Retrieve lists of users and account information to manage access.

### How it works

1. Subscribe to this server
2. Enter your Bounsel API Key
3. Start managing your contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Operations** — quickly check contract statuses and send for signature without navigating the portal.
- **Sales Teams** — generate customized NDAs and sales agreements straight from their workflow tools.
- **HR Managers** — automate employee contract generation using natural language.


## Available Tools (9)
- **create_document**: Create a new document from a template
- **delete_document**: Delete a document
- **get_account_info**: Get company account info
- **get_document**: Get details of a specific document
- **get_template**: Get details of a specific template
- **list_documents**: List all CLM documents
- **list_templates**: List all smart templates
- **list_users**: List all account users
- **send_document**: Send a document for signature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bounsel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active documents in Bounsel."

**🤖 AI Agent:**
> I've retrieved your documents. You have 5 recent files, including 'NDA - Acme Corp' (ID: doc_1) and 'Employment Agreement - Jane' (ID: doc_2).

---

**👤 You:**
> "Send document doc_1 for signature."

**🤖 AI Agent:**
> Document 'doc_1' has been successfully sent for signature. The recipients will receive an email shortly.

---

**👤 You:**
> "List available smart templates."

**🤖 AI Agent:**
> Retrieving templates... You have 3 templates: 'Standard NDA' (ID: tpl_1), 'Sales Contract' (ID: tpl_2), and 'Offer Letter' (ID: tpl_3).


## ❓ FAQ

**Q: Can I automatically generate a contract from a template?**
Yes! Use the `create_document` tool. Provide the Template ID, a name for the new file, and a JSON string containing the data to fill into the template's fields.

**Q: How do I send a completed document for signature?**
Simply ask the agent to `send_document` and provide the Document ID. It will trigger Bounsel's signature workflow for all defined recipients.

**Q: Can I delete a draft document?**
Yes. Use the `delete_document` action with the Document ID to permanently remove it from your Bounsel workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bounsel](https://vinkius.com/mcp/bounsel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bounsel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bounsel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bounsel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bounsel": {
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
