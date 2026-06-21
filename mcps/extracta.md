# Extracta MCP Server

Automate data extraction via Extracta — process documents into structured JSON, handle AI classification, and audit extraction history directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/extracta)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 10

## Description
Connect your **Extracta.ai** account to any AI agent and take full control of your automated data extraction and document classification through natural conversation.

### What you can do

- **Extraction Orchestration** — Create and configure new data extraction processes by defining JSON schemas for fields like dates, amounts, and item descriptions natively
- **Live Document Processing** — Submit publicly accessible file URLs (PDF, JPG, PNG) to trigger asynchronous extraction workflows and retrieve structured JSON data seamlessly
- **AI Classification** — Set up document classification rules to automatically sort documents into types like invoices, receipts, or contracts based on AI predictions
- **Result Auditing** — Retrieve extraction status and finalized structured data for specific documents, evaluating confidence scores and predicted categories flawlessly
- **Batch History Monitoring** — Fetch paginated lists of previously extracted documents and their associated data payloads to track historical processing limitlessly
- **Configuration Mutation** — Update existing extraction settings and mapping rules without creating new endpoints to refine your data parsing logic
- **Workflow Management** — View and manage extraction and classification configurations, including configured fields and webhook settings securely

### How it works

1. Subscribe to this server
2. Enter your Extracta.ai API Key (found in the /api section of your dashboard)
3. Start extracting data from your documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — automate invoice and receipt processing by extracting structured data using natural language
- **Data Analysts** — convert document-based data into JSON formats for analysis without manual data entry
- **Developers** — test and debug data extraction schemas and verify AI classification results through natural conversation
- **Finance Teams** — audit document extraction history and verify data accuracy in real-time


## Available Tools
- **create_classification**: g. invoice, receipt, contract). Pass JSON schema defining categories.

Create a new Extracta document classification setup
- **view_classification**: View details of an existing document classification process
- **get_batch_results**: Get bulk historical results from an Extraction process
- **get_classification_results**: Get the predicted document category from Extracta
- **create_extraction**: g. language, format, expected fields like invoice_date, total_amount). Returns a new extractionId used for subsequent document processing.

Create a new Extracta.ai data extraction process
- **delete_extraction**: Subsequent uploads to this extractionId will fail.

Delete an Extracta.ai extraction process
- **get_results**: If not completed, it will indicate processing status.

Get extraction results for a specific document
- **update_extraction**: Modifies mapping rules without needing to create a new endpoint.

Update an existing Extracta extraction configuration
- **upload_file_url**: Returns a documentId. Use ea.get_results to poll for extracted data.

Upload a document URL to Extracta for processing
- **view_extraction**: View configuration of an existing Extracta extraction process


## Installation & Usage

To install and use the **Extracta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/extracta](https://vinkius.com/mcp/extracta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
