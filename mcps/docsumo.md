# DocSumo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docsumo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docsumo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docsumo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Equip your AI agent to automate document data extraction, manage IDP workflows, and audit processed files via the DocSumo API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocSumo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all processed bank statements."

**🤖 AI Agent:**
> I've found 12 processed bank statements, including 'Chase_June_2023.pdf' and 'Wells_Fargo_Q2.pdf'. Would you like to see the extracted summary for the most recent one?

---

**👤 You:**
> "Show me the extraction results for document 'DOC-5544'."

**🤖 AI Agent:**
> I've retrieved the data for 'DOC-5544'. Extracted fields include: Invoice Number (INV-789), Vendor (Cloud Services Inc), and Grand Total ($4,500.00) with 98% confidence. Should I list the individual line items?

---

**👤 You:**
> "Are there any documents that failed to process today?"

**🤖 AI Agent:**
> I've checked the pipeline and found 2 documents with processing errors: 'Unreadable_Scan.pdf' and 'Wrong_Format.jpg'. Would you like the detailed error messages for these items?


## Installation & Usage

To install and use the **DocSumo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docsumo](https://vinkius.com/mcp/docsumo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
