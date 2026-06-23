# Zoho Sign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-sign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage digital signatures, document requests, and templates via Zoho Sign directly from your AI agent.

## Description
Empower your AI agent with access to the **Zoho Sign** platform to automate your digital signature workflows and document compliance through natural conversation.

### What you can do

- **Signature Request Management** — List all digital signature requests, monitor recipient status, and trigger reminders programmatically.
- **Template Automation** — Create and send document signature requests using reusable templates and pre-configured actions.
- **Compliance & Auditing** — Retrieve legally binding completion certificates and audit trails for signed documents.
- **Document Control** — List supported document types, field types, and access detailed document metadata directly through natural language.

### How it works

1. Subscribe to this server
2. Enter your Zoho Sign Access Token from your developer dashboard
3. Start managing your digital signatures from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & HR Teams** — quickly send employment contracts or legal agreements for signature via natural conversation.
- **Sales Professionals** — monitor contract statuses and remind clients to sign without leaving your workspace.
- **Business Administrators** — automate document workflows and verify signature authenticity efficiently.


## Available Tools (12)
- **create_request_from_template**: Create a sign request from a template
- **get_zohosign_account_info**: Get account profile and settings
- **get_completion_certificate**: Retrieve the audit completion certificate
- **get_document_metadata**: Get metadata for a specific document
- **get_sign_request_details**: Get details for a signature request
- **list_supported_document_types**: g., PDF, DOCX).

List supported file extensions
- **list_available_field_types**: g., Signature, Text, Date) that can be added to documents.

List supported sign fields
- **list_sign_requests**: List all digital signature requests
- **list_sign_templates**: List reusable document templates
- **remind_sign_recipients**: Send reminder to signers
- **revoke_sign_request**: Revoke an active signature request
- **submit_sign_request**: Submit a request for signature


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Sign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active signature requests and send a reminder to any recipients who haven't signed yet."

**🤖 AI Agent:**
> I found 4 active requests. The document 'Partnership Agreement' (ID: 390218) is still pending signature from John Doe. I have successfully sent a reminder notification to John.

---

**👤 You:**
> "Retrieve the completion certificate for the signed document with ID 8493021."

**🤖 AI Agent:**
> I've retrieved the completion certificate for the 'Employment Contract' (ID: 8493021). The document was fully signed and sealed on October 24th. Here is the link to download the legal audit trail.

---

**👤 You:**
> "List all reusable sign templates and initiate a new signature request using the 'NDA Template' (ID: 29013)."

**🤖 AI Agent:**
> You have 5 templates available. I have created a new draft signature request using the 'NDA Template' (ID: 29013). The new request ID is 409122. Let me know when you're ready to submit it.


## ❓ FAQ

**Q: How do I generate an Access Token for Zoho Sign?**
Log in to the [**Zoho API Console**](https://api-console.zoho.com/), register your application, and use the 'Self-Client' option to generate an Access Token with the required Zoho Sign scopes.

**Q: Can the agent send reminders to recipients who haven't signed yet?**
Yes! The `remind_sign_recipients` tool allows your AI agent to trigger a notification to everyone who is still pending to sign the document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-sign](https://vinkius.com/mcp/zoho-sign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Sign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-sign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Sign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-sign": {
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
