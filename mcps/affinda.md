# Affinda MCP Server

Intelligent document processing — parse resumes, invoices, and IDs via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/affinda)

## Overview
**Category:** productivity
**Tools Count:** 5

## Description
Connect your **Affinda** account to your AI agent to unlock powerful intelligent document processing (IDP). From automatically extracting details from resumes and invoices to auditing document statuses across your workspaces, your agent handles structured data extraction through natural conversation.

### What you can do

- **Automated Document Parsing** — Upload PDFs or images of resumes, invoices, and passports for high-accuracy JSON extraction
- **Workspace Oversight** — List and audit documents within your specific workspaces to maintain organizational control
- **Extraction Model Management** — List available document types (Resume, Invoice, Receipt, etc.) supported by your account
- **Real-time Status Tracking** — Retrieve the parsing status and technical metadata for any uploaded document
- **Metadata Insights** — Quickly identify processing errors or missing data across your document library directly from chat

### How it works

1. Subscribe to this server
2. Enter your Affinda Bearer Token
3. Start parsing documents and managing your workspaces through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruitment Teams** — automate resume screening and extract candidate metadata effortlessly
- **Accounts Payable** — audit invoice data extraction and verify payment details via AI
- **Operations Managers** — monitor document processing workflows and manage workspace settings
- **Compliance Officers** — retrieve parsed identity documents for risk assessment and verification


## Available Tools
- **list_documents**: Retrieve all parsed documents in an Affinda workspace with their processing status
- **get_document**: Retrieve the fully structured JSON data and status for a specific processed document in Affinda
- **create_document**: Defaults to synchronous waiting for the output.

Upload and parse a PDF or image into Affinda via its public URL for high-accuracy JSON extraction
- **list_workspaces**: Retrieve all container workspaces for documents created within your Affinda account
- **list_document_types**: Retrieve exactly which parsing models the Affinda account supports (e.g. Resume, Invoice, Passport)


## Installation & Usage

To install and use the **Affinda** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/affinda](https://vinkius.com/mcp/affinda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
