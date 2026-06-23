# Parseur MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/parseur)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate document processing via Parseur — list mailboxes, upload PDFs/Emails, extract structured data pipelines, and trigger template logic natively.

## Description
Bring **Parseur Document Extraction** arrays directly into your AI workflows. By explicitly mapping into powerful OCR and templating engines, your agent can push unstructured PDFs or bulk emails into remote routing limits, parsing exact text fields securely. Extract fields, examine documents, list defined parse-templates, and retry pipelines without manual intervention.

### What you can do

- **Mailboxes & Templates** — Examine specifically bound mailboxes tracking which explicit templates dictate data extraction limits mapped natively 
- **Document Navigation** — Extract properties showing precisely which unstructured strings were identified inside uploaded payloads checking `status: parsed` correctly
- **Payload Uploading** — Instruct the node limits mapping `upload_document` generating raw payloads routing straight into the engine for OCR logic
- **Job Management** — Discover disconnected states mitigating failed validations by pushing `retry_document` instantly forcing physical pipeline resets

### How it works

1. Subscribe to this server
2. Enter your Parseur API Key explicitly
3. Start evaluating explicit AI OCR workflows reliably via Claude, Cursor, or any MCP structure

### Who is this for?

- **Operational Workflows** — explicitly map invoicing pipelines investigating extraction errors remotely avoiding web limits
- **Finance Teams** — trace OCR receipts dynamically identifying missing fields from Chat architectures directly into a JSON limit natively
- **Developers** — route manual document loads simulating continuous AI logic mapping testing integrations on webhook bounds


## Available Tools (10)
- **create_mailbox**: The type determines the parsing engine (e.g., "pdf", "email", "attachment"). Once created, you can configure templates and forward documents to the mailbox for automatic extraction.

Create a new Parseur mailbox for document parsing
- **create_template**: Pass the template name and a JSON config string defining field mappings. Parseur will use this template to extract structured data from matching documents.

Create a new extraction template for a Parseur mailbox
- **get_document_data**: Fields depend on the template configuration (e.g., invoice_number, total_amount, line_items). Only works for documents with status "processed".

Retrieve the fully extracted JSON data from a parsed document
- **get_document_details**: Does not include the parsed data itself — use get_document_data for that.

Get metadata of a single parsed document
- **get_mailbox**: Use this to verify mailbox setup before sending documents.

Get detailed configuration of a specific Parseur mailbox
- **list_documents**: Each entry includes document ID, status (processed, failed, pending), and metadata like sender and received date.

List all parsed documents inside a Parseur mailbox
- **list_mailboxes**: Each mailbox represents a parsing pipeline for a specific document type (invoices, receipts, emails). Use the returned mailbox IDs for subsequent operations like listing documents or uploading files.

List all Parseur parsing mailboxes
- **list_templates**: Templates define the extraction rules (field names, locations, regex patterns) used to pull structured data from incoming documents.

List available extraction templates for a Parseur mailbox
- **retry_document**: Useful after fixing template rules or when the original parse failed due to a transient error. The document will be matched against the latest template rules.

Retry parsing a failed or errored Parseur document
- **upload_document**: eml) to the specified mailbox for automatic parsing. The document enters the processing queue and will be parsed according to the mailbox template. Returns the new document ID for tracking.

Upload a document URL to a Parseur mailbox for parsing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parseur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my Parseur mailboxes to find the specific bounding IDs."

**🤖 AI Agent:**
> Extracted physical boundaries querying mailboxes. I found 2 limits explicitly registered: 1. 'Invoices Mailbox' (ID: xyz12), expecting PDF accounting payloads. 2. 'Web contact forms' (ID: wtf9). Should I list templates associated cleanly?

---

**👤 You:**
> "Get the data schema parsed tightly inside document doc_987."

**🤖 AI Agent:**
> Running payload bounds against doc_987. Status: parsed perfectly. Extracted JSON dictionary properties explicitly reveal: Invoice_Number: 'A-201', Total_Amount: 1400.99, Date: '2026-04-10'.

---

**👤 You:**
> "Upload this snippet of parsed text directly into Mailbox xyz12 for OCR processing."

**🤖 AI Agent:**
> Push executed successfully running `upload_document`. Triggered physical limits. The document natively entered 'Invoices Mailbox' parsing queue. Processing document UUID: doc_112. Status: pending. I'll dynamically pull it later if told.


## ❓ FAQ

**Q: Does this tool parse the document directly or use the cloud engine?**
The tool offloads the logic specifically via endpoints mapping back to the Parseur Cloud Engine. The AI acts to organize mailboxes, list templates, and fetch final states securely without computing massive local OCR networks.

**Q: Can I upload a raw file string to be parsed?**
Yes. Utilizing the explicitly mapped `upload_document` constraint, the agent can inject raw string boundaries identifying formatting, passing files straightforward into the target mailbox ID natively.

**Q: Will I see missing required fields if extraction fails?**
Absolutely. Querying `get_document_details` lists specific status bounds. If a template expects InvoiceTotal and misses it, the document flags a processing boundary issue precisely traceable here.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parseur](https://vinkius.com/mcp/parseur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parseur** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parseur` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parseur** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parseur": {
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
