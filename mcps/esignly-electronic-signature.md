# eSignly Electronic Signature MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esignly-electronic-signature)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Equip your AI agent to manage e-signature documents, track templates, and monitor audit trails via the eSignly API.

## Description
Integrate **eSignly**, the powerful and secure electronic signature platform, directly into your AI workflow. Manage your e-signature documents and reusable templates, track signing statuses and individual signer progress, monitor detailed audit trails and security logs, and oversee your document management using natural language.

### What you can do

- **Document Oversight** — List and retrieve detailed information, sender details, and real-time signing status for all your eSign documents.
- **Template Intelligence** — Monitor reusable document templates, resolving field definitions and placeholder roles across your library.
- **Security Management** — Access and monitor complete document audit trails, identifying signing events, timestamps, and IP addresses.
- **Signing Auditing** — Retrieve high-level summaries of document volume, template usage, and organizational signing health instantly.

### How it works

1. Connect the eSignly integration to your AI assistant.
2. Authorize using your eSignly API ID and API Key (found in your developer settings).
3. Orchestrate your electronic signatures and document workflows through intuitive conversation.

### Who is this for?

- **Legal & Compliance Teams** — Quickly check document audit trails and completion statuses on the go.
- **Sales Operations** — Research active contract statuses and signer progress via chat during deal tracking.
- **HR & Admin Teams** — Monitor template usage and organizational document metadata instantly.


## Available Tools (10)
- **get_template_details**: Get detailed settings for a specific eSign template
- **list_successfully_signed_documents**: Identify documents that have been signed by all parties
- **list_esign_contacts**: List all contacts registered in your eSignly address book
- **list_document_audit_trail**: Get the complete audit trail for a specific document
- **get_esignly_account_metadata**: Retrieve metadata and limits for your eSignly account
- **quick_signing_volume_audit**: Retrieve a high-level summary of document and template activity
- **list_document_signers**: List all signers and their current signing status for a document
- **list_esign_documents**: List all documents in your eSignly account
- **list_esign_templates**: List all reusable document templates
- **get_document_detailed_data**: Get detailed settings and status for a specific document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eSignly Electronic Signature** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all documents awaiting signature."

**🤖 AI Agent:**
> I've found 5 documents awaiting signature, including 'Service Agreement - Q2' and 'Employment Offer - Jane Doe'. 3 signers are still pending for the Service Agreement. Would you like to see the signer details?

---

**👤 You:**
> "Show me the audit trail for document ID 'DOC-12345'."

**🤖 AI Agent:**
> For document 'DOC-12345', I've retrieved the audit trail: Sent at 10:00 AM, Viewed by Signer 1 at 10:15 AM, Signed by Signer 1 at 10:30 AM. Status is 'Partially Signed'. Should I pull the IP addresses for these events?

---

**👤 You:**
> "Search for documents related to 'Project X'."

**🤖 AI Agent:**
> I've found 3 documents matching 'Project X': 'Project X SOW', 'NDA - Project X', and 'Vendor Terms - Project X'. The SOW is 'Completed', while the others are 'Sent'. Would you like the details for the NDA?


## ❓ FAQ

**Q: How do I get eSignly API credentials?**
Log in to your eSignly account, navigate to **Settings > API**, and you can find your unique **API ID** and **API Key** there. Ensure you have a plan that includes API access.

**Q: Can the agent send new documents for signature?**
This integration currently focuses on listing and auditing documents, templates, and contacts. Creating or sending new documents for signature should be managed via the eSignly web portal or automated template triggers.

**Q: Does the integration show real-time signing status?**
Yes, you can use the list_document_signers tool to retrieve the current completion status for every signer associated with a specific document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esignly-electronic-signature](https://vinkius.com/mcp/esignly-electronic-signature)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eSignly Electronic Signature** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `esignly-electronic-signature` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eSignly Electronic Signature** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "esignly-electronic-signature": {
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
