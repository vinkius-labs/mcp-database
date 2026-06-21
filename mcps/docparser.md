# Docparser MCP Server

Equip your AI agent to extract data from documents, manage parsers, and track extraction results via the Docparser API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docparser)

## Overview
**Category:** productivity
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Docparser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docparser](https://vinkius.com/mcp/docparser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
