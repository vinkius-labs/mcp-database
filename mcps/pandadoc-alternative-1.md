# PandaDoc MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pandadoc-alternative-1)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pandadoc-alternative-1-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pandadoc-alternative-1-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Automate document workflows—create from templates, send for signature, and track status directly from your AI agent.

## Description
Connect your **PandaDoc** account to any AI agent to automate your entire document lifecycle—from generation to e-signature—using natural language.

### What you can do

- **Document Creation** — Generate new documents from existing templates or public PDF URLs with custom tokens and fields.
- **Sending & Delivery** — Send documents to recipients with custom email subjects and messages once they are ready.
- **Status Tracking** — Monitor the real-time progress of documents (draft, sent, viewed, completed) and fetch full metadata.
- **Template Management** — List and inspect available templates to ensure you are using the correct version for your contracts.
- **Organization** — Create folders to keep your document workspace structured and manageable.

### How it works

1. Subscribe to this server
2. Enter your PandaDoc API Key
3. Start generating and sending contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — generate and send proposals or quotes instantly after a meeting without leaving the chat.
- **Legal & HR** — track the status of NDAs or employment contracts and download signed versions automatically.
- **Operations** — automate repetitive document workflows by connecting your AI agent to your template library.


## Available Tools
- **create_document_folder**: Create a new folder for documents
- **create_document**: Wait for document.draft status before sending.

Create a new PandaDoc document from a template or URL
- **create_embedded_session**: Create an embedded signing session for a document
- **create_template_folder**: Create a new folder for templates
- **create_webhook_subscription**: Create a webhook subscription for document events
- **download_document**: Download the final signed PDF of a document
- **get_document_details**: Get full document data including fields, tokens, and recipient info
- **get_document_status**: Get current status and basic metadata of a document
- **get_template_details**: Get details of a specific template
- **list_document_folders**: List document folders
- **list_documents**: List PandaDoc documents
- **list_template_folders**: List template folders
- **list_templates**: List PandaDoc templates
- **send_document**: draft status.

Send a PandaDoc document to recipients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PandaDoc** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available PandaDoc templates."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 active templates: 'Sales Proposal' (ID: tp_123), 'NDA Standard' (ID: tp_456), and 'Service Agreement' (ID: tp_789). Which one would you like to use?

---

**👤 You:**
> "Create a document named 'Project Alpha Agreement' using template tp_123 for recipient john@example.com."

**🤖 AI Agent:**
> The document 'Project Alpha Agreement' has been created in draft mode (ID: doc_987). Once you're ready, I can send it to John for signature.

---

**👤 You:**
> "Download the final signed PDF for document doc_987."

**🤖 AI Agent:**
> I've processed the download request for the completed document. You can access the final signed PDF here: [Link].


## Installation & Usage

To install and use the **PandaDoc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pandadoc-alternative-1](https://vinkius.com/mcp/pandadoc-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
