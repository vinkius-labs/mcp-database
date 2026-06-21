# PandaDoc MCP Server

Create, send, and track documents, proposals, and e-signatures via PandaDoc — manage the entire document lifecycle from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pandadoc)

## Overview
**Category:** document-management
**Tools Count:** 10

## Description
Connect your **PandaDoc** account to any AI agent and automate your document workflows through natural conversation.

### What you can do

- **Documents** — List, create from templates, send for signature, check status, and track viewed/completed/declined documents
- **Templates** — Browse all available document templates (proposals, contracts, NDAs, quotes)
- **E-Signatures** — Send documents for signature and monitor signing progress in real time
- **Contacts** — Manage recipient contacts with email, name, and company
- **Team** — List workspace members and their roles

### How it works

1. Subscribe and enter your PandaDoc API key (from **Settings → Integrations → API & Webhooks**)
2. Your AI agent connects to your PandaDoc workspace
3. Ask questions like "create a proposal for Acme" or "who hasn't signed the NDA?"

### Who is this for?

- **Sales Teams** — Create and send proposals, quotes, and contracts without leaving your conversation
- **Operations Managers** — Track document pipeline, follow up on pending signatures, and close deals faster
- **Founders & Freelancers** — Send professional proposals and contracts to clients in seconds


## Available Tools
- **pandadoc_create_contact**: Email is required. Once created, patients can be used as recipients in document creation. Returns the created contact with their PandaDoc ID.

Create a new contact in PandaDoc with email, name, and company for use as a document recipient
- **pandadoc_create_document**: templateId is required (use pandadoc_list_templates to find). Recipients array must include at least email and optionally first_name, last_name, and role (matching template roles). The document is created in "uploaded" status and transitions to "draft" within 3-5 seconds. Fields is an optional JSON object to pre-fill template tokens/variables.

Create a new PandaDoc document from a template with recipients, custom fields, and pricing — ready to send for signature
- **pandadoc_delete_document**: This is irreversible. Only documents in draft or voided status should typically be deleted. Completed/signed documents should be voided first if deletion is required for compliance reasons.

Permanently delete a PandaDoc document — this action cannot be undone and removes the document from all views
- **pandadoc_document_status**: Returns current status, last viewed/completed dates, and recipient progress. Use for tracking: "has the client signed?", "did they view it?", or status polling after sending.

Check the current status of a PandaDoc document — whether it is draft, sent, viewed, completed, or declined
- **pandadoc_get_document**: Returns document name, status, all recipients with their signing status, template reference, pricing table totals, custom field values, and metadata. Use after listing documents to drill into a specific document for complete information.

Get complete details of a specific PandaDoc document by ID, including recipients, fields, tokens, pricing, and audit trail
- **pandadoc_list_contacts**: Returns contact name, email, company, and metadata. Contacts are the people your organization sends documents to. Use when the user asks about recipients, needs to find a contact email, or wants to review the contact database.

List PandaDoc contacts with names, emails, companies, and associated document history
- **pandadoc_list_documents**: Filter by status: draft (not yet sent), sent (awaiting signatures), completed (fully signed), viewed (opened by recipient), paid, voided, or declined. Returns document name, template used, status, total value, owner email, and dates. Use when the user asks about document pipeline, pending signatures, or completed agreements.

List PandaDoc documents with name, status (draft/sent/completed/viewed/paid/voided/declined), creation date, and recipient info
- **pandadoc_list_members**: Returns member name, email, role, and status. Use when the user asks about team members, document ownership, or needs to audit workspace access.

List workspace members (users) in your PandaDoc organization with their email, role, and access level
- **pandadoc_list_templates**: Returns template name, UUID (needed for pandadoc_create_document), creation date, and folder. Templates are reusable document blueprints with pre-defined layouts, fields, and recipient roles. Use when the user asks "what templates do we have?" or needs a template ID before creating a document.

List all PandaDoc templates available for document creation — proposals, contracts, agreements, NDAs, and more
- **pandadoc_send_document**: This triggers email notifications to all recipients. Set silent=true to suppress emails (useful when embedding signing in your own app). An optional message can be included in the notification email. The document moves to "sent" status after this call.

Send a PandaDoc document for signature — transitions it from draft to sent and notifies all recipients via email


## Installation & Usage

To install and use the **PandaDoc** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pandadoc](https://vinkius.com/mcp/pandadoc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
