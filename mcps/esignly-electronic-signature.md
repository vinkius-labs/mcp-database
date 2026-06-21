# eSignly Electronic Signature MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esignly-electronic-signature)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/esignly-electronic-signature-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/esignly-electronic-signature-mcp)
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


## Available Tools
- **get_esignly_account_metadata**: Retrieve metadata and limits for your eSignly account
- **get_document_detailed_data**: Get detailed settings and status for a specific document
- **quick_signing_volume_audit**: Retrieve a high-level summary of document and template activity
- **get_template_details**: Get detailed settings for a specific eSign template
- **list_successfully_signed_documents**: Identify documents that have been signed by all parties
- **list_esign_contacts**: List all contacts registered in your eSignly address book
- **list_document_audit_trail**: Get the complete audit trail for a specific document
- **list_document_signers**: List all signers and their current signing status for a document
- **list_esign_documents**: List all documents in your eSignly account
- **list_esign_templates**: List all reusable document templates


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


## Installation & Usage

To install and use the **eSignly Electronic Signature** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esignly-electronic-signature](https://vinkius.com/mcp/esignly-electronic-signature)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
