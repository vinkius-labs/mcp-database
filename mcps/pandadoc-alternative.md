# PandaDoc MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pandadoc-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Close deals faster with proposals, contracts, and e-signatures in one platform that tracks document engagement in real time.

## Description
Connect your **PandaDoc** account to any AI agent and take full control of your document orchestration and e-signature workflows through natural conversation. PandaDoc provides a premier platform for creating, sending, and tracking business documents, and this integration allows you to retrieve document metadata, monitor signature statuses, and generate new contracts directly from your chat interface.

### What you can do

- **Document & Signature Orchestration** — List all managed documents and retrieve detailed status metadata programmatically to ensure your sales closing is always synchronized.
- **Template Lifecycle Management** — Access and monitor your centralized template library and retrieve detailed metadata for dynamic field mapping directly from the AI interface.
- **Contract & Proposal Control** — Create new documents from existing templates and send them to multiple recipients with personalized messages via natural language.
- **Embedded Signing Intelligence** — Generate embedded signing sessions for real-time customer signatures and retrieve direct download links for final PDFs using simple AI commands.
- **Operational Monitoring** — Track system responses and manage document folders to ensure your administrative workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your PandaDoc API Key from your integration settings
3. Start managing your document automation from Claude, Cursor, or any MCP-compatible client

No more manual status checking or template searching. Your AI acts as a dedicated document coordinator or sales operations assistant.

### Who is this for?

- **Sales Teams** — quickly retrieve contract statuses and send new proposals without switching apps.
- **HR Managers** — automate the issuance of onboarding documents and track signing progress via natural conversation.
- **Operations Teams** — streamline the retrieval of document metadata and monitor organizational health directly within the chat.


## Available Tools (11)
- **create_document**: Requires a JSON string containing "template_uuid" and "recipients" list. Use this to initiate the document creation process.

Create a new PandaDoc document
- **create_signing_session**: Create an embedded signing session
- **delete_document**: Delete a PandaDoc document
- **get_download_link**: Get the download link for a completed document
- **get_document_details**: Essential for tracking the progress of an individual signature request.

Get details for a specific document
- **get_template_details**: Get details for a specific template
- **list_contacts**: List all contacts in PandaDoc
- **list_documents**: Supports searching by query (q) and filtering by status (e.g., document.draft, document.sent). Useful for monitoring the status of multiple agreements.

List all PandaDoc documents
- **list_folders**: Useful for navigating the account structure.

List document organization folders
- **list_templates**: Essential for obtaining the template IDs required for document creation.

List all document templates
- **send_document**: Can include an optional message to be sent in the notification email.

Send a document for signing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PandaDoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my PandaDoc documents and their statuses."

**🤖 AI Agent:**
> I've retrieved your documents. You have 15 active files including 'Acme Contract' (Status: draft) and 'Renewal Proposal' (Status: sent). Would you like to check the recipient for any of them?

---

**👤 You:**
> "Send the contract document doc_3847 to the client for electronic signature."

**🤖 AI Agent:**
> Document doc_3847 "Service Agreement 2025" has been sent for signature. Recipients: John Martinez (CEO) at john@acmecorp.com and Lisa Park (Legal) at lisa@acmecorp.com. Both received email notifications with unique signing links. The document status has changed from Draft to Sent. Average completion time for similar documents is 2.3 days.

---

**👤 You:**
> "List all available document templates I can use to create new proposals."

**🤖 AI Agent:**
> You have 12 templates available. Top 5 by usage: "Standard SaaS Agreement" (used 34 times), "Consulting Proposal" (28 uses), "NDA Mutual" (22 uses), "Statement of Work" (18 uses), and "Sales Quote" (15 uses). 3 templates were updated in the last 30 days. All templates support dynamic field merging with recipient and company data.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific document by its ID?**
Yes! Use the `get_document` tool with the Document ID. Your agent will respond with complete metadata, including signature status, expiration dates, and recipient info in seconds.

**Q: How do I find my PandaDoc API Key?**
Log in to your PandaDoc account, navigate to **Settings** > **Integrations** > **API**, and click 'Generate API Key' to create your unique secret token.

**Q: Can I generate a signing link for my app?**
Absolutely. Use the `create_session` tool to generate an embedded signing session for a specific document. The agent will return a unique URL for your recipient to sign immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pandadoc-alternative](https://vinkius.com/mcp/pandadoc-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PandaDoc** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pandadoc-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PandaDoc** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pandadoc-alternative": {
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
