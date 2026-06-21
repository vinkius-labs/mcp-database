# SignRequest MCP Server

Manage e-signatures and documents via SignRequest — create signing requests, track document status, and manage templates directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/signrequest)

## Overview
**Category:** productivity
**Tools Count:** 12

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


## Installation & Usage

To install and use the **SignRequest** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signrequest](https://vinkius.com/mcp/signrequest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
