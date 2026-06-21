# Docupilot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docupilot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docupilot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docupilot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to automate document creation, manage templates, and track merges via the Docupilot API.

## Description
Integrate **Docupilot**, the powerful document automation platform, directly into your AI workflow. Manage your dynamic document templates, trigger high-volume document merges from JSON data, monitor generation status, and access output files using natural language.

### What you can do

- **Template Oversight** — List and retrieve detailed configuration and field schemas for all your document templates.
- **Document Merging** — Trigger the Docupilot engine to create new files by merging provided data into your professional templates.
- **Generation Tracking** — Monitor the status of your document merges and access secure download URLs for output files.
- **Field Intelligence** — Identify exactly which merge fields are required to populate specific templates accurately.

### How it works

1. Connect the Docupilot integration to your AI assistant.
2. Authorize using your Docupilot API Key (found in your account settings).
3. Orchestrate your document automation and reporting through intuitive conversation.

### Who is this for?

- **Sales & Marketing** — Quickly generate personalized proposals or contracts from CRM data on the go.
- **HR Teams** — Monitor employee document generation and access output files via chat.
- **Developers** — Audit merge fields and test document automation workflows instantly.


## Available Tools
- **trigger_document_merge**: Create a new document by merging data into a specific template
- **get_docupilot_account_metadata**: Retrieve metadata and usage limits for your Docupilot account
- **get_document_generation_status**: Get the current status and output URL for a specific generated document
- **get_template_merge_field_audit**: Identify exactly which merge fields are required to populate a template
- **get_template_schema**: Get detailed information and field schema for a specific template
- **list_generated_documents**: List all documents that have been generated/merged in Docupilot
- **list_failed_document_merges**: Identify document merges that failed due to data or template errors (mock logic)
- **list_latest_document_merges**: Identify the most recently merged documents
- **list_docupilot_templates**: List all document templates available in your Docupilot account
- **search_docupilot_templates**: Search for a document template using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docupilot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available Docupilot templates."

**🤖 AI Agent:**
> I've found 6 templates in your account, including 'Standard Service Contract', 'Monthly Performance Dashboard', and 'Employee Offer Letter'. Would you like to see the merge fields for the Service Contract?

---

**👤 You:**
> "Generate an 'Employee Offer Letter' with data: {'name': 'Robert Brown', 'role': 'Engineer', 'salary': '90k'}."

**🤖 AI Agent:**
> I've triggered the merge for 'Employee Offer Letter'. The document is currently being generated. I'll provide the download URL shortly. The document ID is 'DOCU-MERGE-12345'.

---

**👤 You:**
> "Show me the status of document 'DOCU-MERGE-12345'."

**🤖 AI Agent:**
> Document 'DOCU-MERGE-12345' is now 'Completed'. You can download it here: [https://api.docupilot.app/download/...] (Link expires in 24 hours). Should I list other recently merged documents?


## Installation & Usage

To install and use the **Docupilot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docupilot](https://vinkius.com/mcp/docupilot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
