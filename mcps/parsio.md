# Parsio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/parsio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Extract structured data from emails and PDFs automatically with AI-powered parsing templates that learn from your documents.

## Description
Connect your **Parsio.io** account to any AI agent and take full control of your document automation and data extraction through natural conversation. Parsio provides a powerful AI-powered parsing engine that transforms unstructured PDF files, images, and emails into structured JSON data directly from your chat interface.

### What you can do

- **Document Extraction Orchestration** — Upload files (via URL or raw text) and trigger real-time parsing to retrieve structured metadata programmatically.
- **Mailbox Lifecycle Management** — List all managed mailboxes and retrieve detailed configuration metadata directly from the AI interface to ensure your data pipelines are always synchronized.
- **Template & Parsing Intelligence** — Access and monitor your parsing templates to maintain a clear overview of how your data is being structured via natural language.
- **Historical Data Control** — List collected parsed data from specific mailboxes and retrieve granular details for individual documents using simple AI commands.
- **Operational Monitoring** — Track system responses and manage webhook metadata to ensure your document automation is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Parsio API Key from your account settings
3. Start managing your document parsing from Claude, Cursor, or any MCP-compatible client

No more manual data entry from invoices or forms. Your AI acts as a dedicated document analyst or data processing coordinator.

### Who is this for?

- **Operations Managers** — quickly retrieve parsed summaries from high volumes of forms without switching apps.
- **Finance Teams** — automate the extraction of data from invoices and receipts via natural conversation.
- **Developers** — integrate real-time document parsing and structured data retrieval directly within the chat.


## Available Tools
- **create_mailbox**: Create a new mailbox
- **get_parsed_document_result**: Retrieve the result of a parsed document
- **get_mailbox**: Get details for a specific mailbox
- **get_template_details**: Get template metadata
- **list_mailboxes**: List all Parsio mailboxes
- **list_parsed_data_history**: List historical parsed data for a mailbox
- **list_mailbox_templates**: List parsing templates for a mailbox
- **list_mailbox_webhooks**: List webhooks for a mailbox
- **extract_data_from_text_async**: Start text data extraction (Async)
- **extract_data_from_text_sync**: Extract data from text or HTML (Sync)
- **extract_data_from_file_async**: Use this for large files or webhook workflows.

Start file data extraction (Async)
- **extract_data_from_file_sync**: Extract data from a file immediately (Sync)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parsio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Parsio mailboxes."

**🤖 AI Agent:**
> I've retrieved your mailboxes. You have 3 active containers: 'Sales Invoices', 'Customer Support', and 'Expense Receipts'. Which one would you like to list templates for?

---

**👤 You:**
> "Show me all parsing templates I have configured and their extraction success rates."

**🤖 AI Agent:**
> You have 6 active parsing templates. "Invoice Parser" processes 94% of documents successfully with 12 extracted fields. "Receipt Scanner" has 89% accuracy across 847 documents processed this month. "Purchase Order Template" handles 97% success rate. "Resume Parser" extracts from 91% of uploads. Your total documents processed this month: 3,421.

---

**👤 You:**
> "Get the extracted data from the last 5 invoices processed by my Invoice Parser template."

**🤖 AI Agent:**
> Here are the last 5 invoices processed. Invoice from Acme Corp: $4,250.00, dated May 8, PO#2847. Invoice from TechSupply: $1,890.50, dated May 7, NET30 terms. Invoice from CloudServices: $699.00, recurring monthly. Invoice from OfficeMax: $342.18, supplies category. Invoice from DataCenter Inc: $12,500.00, infrastructure. All 5 extracted with 100% field confidence.


## ❓ FAQ

**Q: Can my AI automatically find the parsed results for a specific invoice URL?**
Yes! Use the `upload_file_sync` tool. Provide the file URL and the Mailbox ID, and your agent will respond with the structured JSON data extracted from the document in seconds.

**Q: How do I find my Parsio API Key?**
Log in to your Parsio account, navigate to **Account Settings** > **API**, and you will find your unique secret API key there.

**Q: Does it support hand-written text recognition?**
Absolutely. Parsio's AI-powered OCR engine is designed to handle both printed and hand-written text from scanned images and PDFs with high accuracy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parsio](https://vinkius.com/mcp/parsio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parsio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `parsio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parsio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parsio": {
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
