# Docparser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docparser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docparser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docparser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to extract data from documents, manage parsers, and track extraction results via the Docparser API.

## Description
Integrate **Docparser**, the leading document data extraction platform, directly into your AI workflow. Automate the extraction of structured data from PDFs, scanned documents, and images, monitor your parser configurations, and retrieve parsed results using natural language.

### What you can do

- **Parser Oversight** — List and retrieve detailed settings and status for all your document parsers and extraction rules.
- **Data Intelligence** — Access the actual structured data extracted from your documents, including table data and custom fields.
- **Document Tracking** — Monitor the processing status of your uploaded documents and identify any extraction failures.
- **Result Auditing** — Retrieve a chronological feed of recent extraction results across all your active parsers.

### How it works

1. Connect the Docparser integration to your AI assistant.
2. Authorize using your Docparser API Key (found in your account settings).
3. Orchestrate your document data extraction and automation through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly retrieve extracted data from invoices or orders on the go.
- **Data Analysts** — Gather structured information from processed documents for reporting via chat.
- **Automation Leads** — Monitor parser health and success rates across the document pipeline instantly.


## Available Tools
- **get_docparser_account_metadata**: Retrieve metadata and usage limits for your Docparser account
- **get_parser_details**: Get detailed settings and status for a specific document parser
- **quick_parser_health_audit**: Retrieve a high-level summary of parser activity and success rates
- **get_document_extraction_results**: Get the actual data extracted from a specific document
- **list_parsed_documents**: List all documents processed by a specific parser
- **list_failed_document_extractions**: Identify documents that failed the parsing or extraction process (mock logic)
- **list_document_parsers**: List all document parsers configured in your Docparser account
- **list_documents_awaiting_parsing**: List documents that are currently in the parsing queue
- **list_recent_extractions**: List the most recent document extraction results across all parsers
- **search_parsed_documents**: Search for parsed documents by filename within a parser


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docparser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all documents processed by the 'Invoices' parser."

**🤖 AI Agent:**
> I've found 15 documents processed by the 'Invoices' parser, including 'Inv_123.pdf' and 'Supplier_A_June.pdf'. Would you like to see the extracted results for the most recent one?

---

**👤 You:**
> "Show me the extracted data for document 'DOC-9988' in the 'Orders' parser."

**🤖 AI Agent:**
> I've retrieved the data for 'DOC-9988'. Extracted fields include: Order Number (ORD-456), Customer (Tech Corp), and Total Amount ($1,250.00). Would you like the full JSON output including line items?

---

**👤 You:**
> "Are there any document extractions that failed today?"

**🤖 AI Agent:**
> I've checked your active parsers and found 2 documents that failed to process: 'BadScan_01.jpg' (Error: Unreadable) and 'UnknownFormat.pdf'. Would you like me to pull the detailed error logs for these?


## Installation & Usage

To install and use the **Docparser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docparser](https://vinkius.com/mcp/docparser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
