# DocSumo MCP Server

Equip your AI agent to automate document data extraction, manage IDP workflows, and audit processed files via the DocSumo API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docsumo)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 10

## Description
Integrate **DocSumo**, the advanced Intelligent Document Processing (IDP) platform, directly into your AI workflow. Automate the extraction of complex data from invoices, bank statements, and ID cards, monitor your processing pipelines, and retrieve structured results using natural language.

### What you can do

- **Pipeline Oversight** — List and retrieve detailed settings and processing statuses for all your document types and IDP workflows.
- **Data Intelligence** — Access the structured data extracted by DocSumo's AI engine, including table layouts and verified fields.
- **Confidence Monitoring** — Identify documents that require manual review due to low extraction confidence scores.
- **Extraction Auditing** — Retrieve a chronological feed of recent extraction results across all your processed document categories.

### How it works

1. Connect the DocSumo integration to your AI assistant.
2. Authorize using your DocSumo API Key (found in your platform settings).
3. Orchestrate your document data extraction and verification through intuitive conversation.

### Who is this for?

- **Finance Teams** — Quickly retrieve extracted data from invoices and receipts for bookkeeping via chat.
- **Compliance Officers** — Audit processed ID cards and bank statements for verification status instantly.
- **Operations Leads** — Monitor document processing health and success rates across the organizational pipeline.


## Available Tools
- **get_docsumo_account_metadata**: Retrieve metadata and usage limits for your DocSumo account
- **get_document_extraction_data**: Get the structured data extracted from a specific document
- **quick_idp_health_audit**: Retrieve a high-level summary of document processing activity and success rates
- **list_successfully_parsed_docs**: Identify documents that have been successfully processed and verified
- **list_docsumo_document_types**: List all document types (e.g., invoices, bank statements) configured in DocSumo
- **list_processed_documents**: List all documents processed by DocSumo, optionally filtered by document type
- **list_failed_doc_extractions**: Identify documents that failed the extraction process (mock logic)
- **list_latest_extraction_results**: Identify the most recently processed documents across all types
- **list_documents_awaiting_review**: Identify documents that require manual review due to low extraction confidence
- **search_documents_by_filename**: Search for processed documents using a filename keyword


## Installation & Usage

To install and use the **DocSumo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docsumo](https://vinkius.com/mcp/docsumo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
