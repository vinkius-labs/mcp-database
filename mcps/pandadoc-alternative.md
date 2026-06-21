# PandaDoc MCP Server

Close deals faster with proposals, contracts, and e-signatures in one platform that tracks document engagement in real time.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pandadoc-alternative)

## Overview
**Category:** industry-titans
**Tools Count:** 11

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


## Available Tools
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


## Installation & Usage

To install and use the **PandaDoc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pandadoc-alternative](https://vinkius.com/mcp/pandadoc-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
