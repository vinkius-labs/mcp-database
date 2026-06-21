# Modusign MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modusign)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/modusign-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/modusign-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage electronic contracts and signatures via Modusign — track documents and request signatures directly from your AI agent.

## Description
Connect your **Modusign** account to your AI agent and streamline your document signing workflows through natural conversation.

### What you can do

- **Document Tracking** — List all electronic contracts and get real-time status updates (e.g., signed, pending).
- **Deep Inspection** — Fetch complete metadata and audit trails for specific documents using their IDs.
- **Template Management** — List your pre-defined contract templates for quick reuse.
- **Signature Requests** — Create new signature requests from templates with a simple natural language command.
- **Automation & Webhooks** — Monitor your automated signature workflows and active webhooks.
- **Org Structure** — Access folders and organization metadata to keep your documents organized.

### How it works

1. Subscribe to this server
2. Enter your Modusign API Key
3. Start managing your contracts from Claude, Cursor, or any MCP client

### Who is this for?

- **Legal & HR Teams** — quickly check which employees or clients have signed their contracts.
- **Sales Teams** — send out signature requests for new deals directly from your CRM or chat tool.
- **Operations** — monitor document workflows and follow up on pending signatures without leaving your workspace.


## Available Tools
- **create_document_from_template**: Create document from template
- **get_audit_logs**: Get document audit logs
- **get_document**: Get specific document details
- **get_org_info**: Get organization metadata
- **list_automations**: List signature automations
- **list_documents**: List electronic documents
- **list_external_files**: List external document files
- **list_folders**: List document folders
- **list_templates**: List contract templates
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Modusign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent electronic documents."

**🤖 AI Agent:**
> I've retrieved your recent documents. You have 5 active contracts, including 'Partnership Agreement' (Status: Signed) and 'Employment Offer - John Doe' (Status: Pending Signature). Would you like the details for any of these?

---

**👤 You:**
> "Send a 'Standard NDA' to ryan@example.com using template ID tmp_123."

**🤖 AI Agent:**
> I've initiated the signature request for the 'Standard NDA'. The document has been created from template tmp_123 and sent to ryan@example.com. The new Document ID is doc_987.

---

**👤 You:**
> "Show me the audit logs for document doc_987."

**🤖 AI Agent:**
> Retrieving audit logs for doc_987... The document was created at 10:00 AM, sent to ryan@example.com at 10:05 AM, and was opened by the participant at 10:15 AM. It is currently awaiting signature.


## Installation & Usage

To install and use the **Modusign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modusign](https://vinkius.com/mcp/modusign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
