# Sensible MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sensible)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Extract structured data from PDFs, images, and documents using Sensible's powerful document parsing engine.

## Description
Connect **Sensible** to your AI agent to seamlessly extract structured data from unstructured documents like PDFs, Word files, and images.

### What you can do

- **Synchronous Extraction** — Extract data instantly from local documents provided as Base64 strings using `extract_sync` or `extract_sync_with_config`.
- **URL-Based Extraction** — Process documents hosted online asynchronously using `extract_from_url` or `extract_from_url_with_config`.
- **Pre-signed Upload URLs** — Generate secure upload URLs for asynchronous document processing using `generate_upload_url`.

### How it works

1. Subscribe to this server
2. Enter your Sensible API Key
3. Start extracting structured JSON from any document directly from your AI agent

### Who is this for?

- **Developers** — Automate document parsing workflows directly from your IDE or terminal.
- **Operations Teams** — Extract data from invoices, tax forms, and contracts without manual data entry.
- **Data Analysts** — Convert unstructured document repositories into clean, structured datasets.


## Available Tools
- **classify_async**: Classify a document into one of the document types asynchronously
- **classify_sync**: Classify a document into one of the document types synchronously
- **create_configuration**: Create a new configuration for a document type
- **create_document_type**: Create a new document type
- **create_golden**: Create a reference document (Golden). Returns an upload URL
- **delete_configuration**: Delete a configuration
- **delete_configuration_version**: Delete a draft or unpublish a configuration version
- **delete_document_type**: Delete a document type
- **delete_golden**: Delete a reference document
- **extract_from_url_with_config**: Extract data from a document at a URL using a specified config asynchronously
- **extract_from_url**: Extract data from a document at a URL asynchronously
- **extract_portfolio_from_url**: Extract data from a portfolio document at a URL asynchronously
- **extract_sync_with_config**: Extract data from a document using a specified config synchronously
- **extract_sync**: Provide the document as a Base64 string.

Extract data from a document synchronously
- **extract_text_from_golden**: Extract all text lines and positioning coordinates from a reference document
- **generate_csv**: Compile JSON document extractions into a CSV spreadsheet
- **generate_excel**: Compile JSON document extractions into an Excel spreadsheet
- **generate_portfolio_upload_url**: Generate a pre-signed upload URL for portfolio extraction
- **generate_upload_url_with_config**: Generate a pre-signed upload URL for asynchronous extraction using a specified config
- **generate_upload_url**: Generate a pre-signed upload URL for asynchronous extraction
- **get_auth_tokens**: Generates a temporary authorization token for external reviewers
- **get_configuration**: Get a specific configuration
- **get_configuration_version**: Get a specific version of a configuration
- **get_document_type**: Get a specific document type
- **get_document**: Retrieve extraction results by ID
- **get_extraction_statistics**: Returns daily extraction coverage statistics
- **get_golden**: Get reference document metadata
- **list_configuration_versions**: List versions of a configuration
- **list_configurations**: List configurations for a document type
- **list_document_types**: List all document types
- **list_extractions**: Retrieve a filtered, paginated list of past extractions
- **list_goldens**: List reference documents for a document type
- **publish_configuration**: Publish a configuration version to an environment
- **unassociate_golden**: Unassociate a reference document from its configuration
- **update_configuration**: Update a configuration
- **update_document_type**: Update a document type
- **update_golden**: Update reference document metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sensible** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract data synchronously from this Base64 PDF using the 'invoice' document type."

**🤖 AI Agent:**
> I've processed the document using `extract_sync`. Here are the extracted fields: Invoice Number: INV-2023-001, Total Amount: $1,250.00, Due Date: December 15, 2023.

---

**👤 You:**
> "Extract data from the document at 'https://example.com/tax_form.pdf' using the 'tax_1099' document type."

**🤖 AI Agent:**
> I have initiated the asynchronous extraction using `extract_from_url`. The document has been submitted to Sensible for processing.

---

**👤 You:**
> "Generate a pre-signed upload URL for a PDF document of type 'bank_statement'."

**🤖 AI Agent:**
> I've generated the upload URL using `generate_upload_url`. You can upload your PDF directly to this secure endpoint to start the extraction process.


## ❓ FAQ

**Q: Can I extract data from a document instantly if I have its Base64 representation?**
Yes! Use the `extract_sync` tool. Provide the document type and the Base64-encoded document bytes, and your agent will return the structured extraction results synchronously.

**Q: How do I extract data from a document hosted at a public URL?**
You can use the `extract_from_url` tool. Simply provide the document type, the document URL, and the content type (e.g., application/pdf) to trigger an asynchronous extraction.

**Q: Can I specify a custom configuration layout when extracting?**
Yes, you can target specific configurations by using the `extract_sync_with_config` or `extract_from_url_with_config` tools, which allow you to define the exact configuration name to use for parsing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sensible](https://vinkius.com/mcp/sensible)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sensible** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sensible` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sensible** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sensible": {
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
