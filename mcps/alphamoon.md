# Alphamoon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alphamoon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Extract data from documents using AI-powered OCR and intelligent document processing for contracts, invoices, and forms.

## Description
Connect your **Alphamoon** account to any AI agent and take full control of your automated document processing and intelligent data extraction workflows through natural conversation.

### What you can do

- **Pipeline Orchestration** — List and manage available document automation pipelines programmatically to coordinate high-fidelity data extraction tasks
- **AI Data Extraction** — Programmatically retrieve structured fields from processed documents (invoices, IDs, etc.) with high-fidelity accuracy and confidence scores
- **Raw OCR Intelligence** — Access the complete high-fidelity recognized text (OCR) from scanned files and PDFs directly through your agent
- **Document Lifecycle Management** — List all processed documents and monitor their status programmatically to maintain a perfectly coordinated audit trail
- **Infrastructure Monitoring** — Verify API connectivity and retrieve account-level metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Alphamoon dashboard (Settings > API)
3. Start automating your document-heavy workflows from Claude, Cursor, or any MCP client

No more manual data entry from complex PDFs or digging through individual extraction logs. Your AI acts as your dedicated document engineer and data architect.

### Who is this for?

- **Operations Managers** — instantly verify extraction results for high-volume batches using natural language commands
- **Financial Analysts** — automate the ingestion of invoice data into custom reports without leaving your workspace
- **Developers** — integrate high-speed document intelligence into custom automation workflows through simple AI queries


## Available Tools
- **check_alphamoon_status**: Verify connectivity
- **delete_document**: Delete a document
- **get_document**: Get document details
- **get_extraction_results**: Get extraction results
- **get_ocr_results**: Get OCR results
- **get_process**: Get process details
- **get_template**: Get template details
- **list_documents_by_process**: List documents by process
- **list_documents**: List documents
- **list_processes**: List processes
- **list_templates**: List templates
- **upload_document**: Upload a document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alphamoon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my document automation pipelines in Alphamoon."

**🤖 AI Agent:**
> I've retrieved your automation directory. You currently have 3 active pipelines: 'Invoice Processing' (ID: pipe_123), 'ID Verification', and 'Receipt OCR'. Which one should we check for processed documents?

---

**👤 You:**
> "Show the extraction results for document ID '90210'."

**🤖 AI Agent:**
> Fetching results... For document 90210, I've identified high-fidelity fields including 'Total Amount' ($250.00), 'Date' (2026-04-24), and 'Vendor Name'. All fields have 99% confidence scores. Need the raw OCR text?

---

**👤 You:**
> "Get the raw OCR text from document '90210'."

**🤖 AI Agent:**
> Accessing OCR data... I've retrieved the complete high-fidelity recognized text from document 90210. It contains 15 paragraphs and includes all detected hand-written notes. Shall I summarize the content for you?


## ❓ FAQ

**Q: How do I find my Alphamoon API Key?**
Log in to your account, navigate to **Settings** > **API**, and generate a new API Key for your integration.

**Q: Can I retrieve raw OCR text via AI?**
Yes! The `get_ocr_results` tool allows your agent to retrieve the complete high-fidelity recognized text from any processed document.

**Q: How do I check extraction results?**
Use the `get_extraction_results` tool and provide the document ID to retrieve structured fields and confidence scores programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alphamoon](https://vinkius.com/mcp/alphamoon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alphamoon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `alphamoon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alphamoon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alphamoon": {
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
