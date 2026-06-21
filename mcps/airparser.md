# Airparser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airparser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/airparser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/airparser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

AI data extraction orchestration — parse PDFs, emails, and images into structured data via AI.

## Description
Connect your **Airparser** account to your AI agent to unlock professional unstructured data extraction and IDP (Intelligent Document Processing). From automatically parsing complex invoices and resumes to auditing extraction schemas and managing automated webhooks, your agent handles your data processing pipeline through natural conversation.

### What you can do

- **Document Parsing** — Upload and parse PDFs, emails (EML/HTML), and images synchronously or asynchronously
- **Inbox Management** — List and audit your Airparser inboxes to organize different document types and sources
- **Schema Orchestration** — Retrieve and verify extraction schemas to ensure your structured data matches your database requirements
- **Automated Workflows** — List and create webhooks to automatically push parsed JSON data to your external applications
- **Real-time Status** — Monitor document processing statuses and retrieve historical parsing results directly from chat

### How it works

1. Subscribe to this server
2. Enter your Airparser API Key
3. Start parsing documents and managing your extraction pipelines through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — automate invoice and receipt processing to streamline accounts payable
- **Recruiters** — parse hundreds of resumes into structured JSON for easier candidate filtering
- **Developers** — integrate GPT-powered document parsing into custom workflows using simple commands
- **Data Analysts** — convert messy unstructured data into clean structured formats for reporting


## Available Tools
- **list_inboxes**: List Airparser inboxes
- **get_inbox_details**: Get inbox metadata
- **parse_document_sync**: Parse document immediately
- **parse_document_async**: Parse document in background
- **list_documents**: List documents in inbox
- **get_document_details**: Get extracted JSON data
- **get_inbox_schema**: Get extraction field definitions
- **list_webhooks**: List inbox webhooks
- **create_webhook**: Add automated data export
- **delete_webhook**: Remove automated export


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airparser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all inboxes in my Airparser account."

**🤖 AI Agent:**
> I've retrieved your inboxes. You have 5 active inboxes, including 'Invoices_US', 'HR_Resumes', and 'Sales_Leads'. Which one would you like to check for recent documents?

---

**👤 You:**
> "Show me the extraction schema for inbox ID 'abc-123'."

**🤖 AI Agent:**
> I've retrieved the schema for inbox abc-123. It is configured to extract 10 fields, including 'VendorName', 'Date', 'TotalAmount', and a table for 'LineItems'. Would you like to see the data types for each field?

---

**👤 You:**
> "Check the status of document ID 'doc_98765'."

**🤖 AI Agent:**
> The status for document doc_98765 is 'Completed'. The data was successfully extracted using the 'Invoice' model. Would you like me to retrieve the full JSON result for you?


## Installation & Usage

To install and use the **Airparser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airparser](https://vinkius.com/mcp/airparser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
