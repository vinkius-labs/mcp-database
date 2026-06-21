# AlgoDocs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/algodocs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

AI document extraction orchestration — parse PDFs, images, and Word docs via AI.

## Description
Connect your **AlgoDocs** account to your AI agent to unlock professional automated document extraction. From automatically parsing invoices, receipts, and complex tables to auditing extraction models (extractors) and managing folder hierarchies, your agent handles your data ingestion pipeline through natural conversation.

### What you can do

- **Document Ingestion** — Upload and parse documents from public URLs or Base64 strings for high-accuracy JSON extraction
- **Extractor Oversight** — List and retrieve details for your AI extractors to ensure the correct rulesets are applied to your docs
- **Data Auditing** — Retrieve structured JSON results for individual documents or list extracted data in bulk for entire extractors
- **Folder Management** — List and audit your folder hierarchy to organize your document processing projects
- **Usage Monitoring** — Quickly retrieve account details and API usage statistics directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AlgoDocs Email and API Key
3. Start parsing documents and managing your extraction workflows through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Finance Teams** — automate data extraction from thousands of invoices and receipts effortlessly
- **Data Entry Specialists** — convert scanned PDFs and images into structured JSON without manual typing
- **Operations Managers** — monitor document processing status and audit extractor accuracy on the fly
- **Developers** — integrate intelligent OCR and data parsing into custom applications using simple commands


## Available Tools
- **get_my_account**: Check account status
- **list_extractors**: List AI extractors
- **list_folders**: List storage folders
- **upload_document_from_url**: Parse document from URL
- **get_document_data**: Get parsed data
- **list_extractor_data**: Bulk extraction results
- **get_document_status**: Check processing status
- **get_folder_details**: Get folder metadata
- **get_api_usage**: Get usage stats
- **list_recent_documents**: List latest parsed docs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AlgoDocs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all extractors in my AlgoDocs account."

**🤖 AI Agent:**
> I've retrieved your extractors. You have 4 active models: 'Invoice_Parser_V2', 'Receipt_Scanner', 'HR_Resumes', and 'Shipping_Labels'. Which one would you like to use for your next document?

---

**👤 You:**
> "Parse this invoice URL: https://example.com/inv.pdf using extractor ID 'ext_123'."

**🤖 AI Agent:**
> I've started the extraction for the document at that URL using extractor ext_123. The unique document identifier is 'doc_98765'. I'll monitor the status and notify you as soon as the structured JSON is ready.

---

**👤 You:**
> "Show the extracted data for document ID 'doc_98765'."

**🤖 AI Agent:**
> I've retrieved the data for document doc_98765. It contains an invoice for $1,250.00 from 'Global Supplies', dated March 15th, 2026. All 5 line items have been correctly identified. Would you like the full JSON payload?


## ❓ FAQ

**Q: How do I find my AlgoDocs API Key?**
Log in to AlgoDocs, go to your **Account Settings**, and you will find your API key there. You will need this along with your registered email for authentication.

**Q: What is an 'Extractor' in AlgoDocs?**
An Extractor is a set of rules and AI models configured to pull specific fields from a certain type of document (e.g., an Invoice Extractor). You must specify an `extractor_id` when uploading documents.

**Q: Can I retrieve data from a previously processed document?**
Yes! Use the `get_document_data` tool and provide the unique `document_id`. Your agent will retrieve the extracted structured data from AlgoDocs storage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/algodocs](https://vinkius.com/mcp/algodocs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AlgoDocs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `algodocs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AlgoDocs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "algodocs": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
