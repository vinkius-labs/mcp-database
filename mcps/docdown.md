# Docdown MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docdown)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to generate documents, manage templates, and track output files via the Docdown API.

## Description
Integrate **Docdown**, the efficient document generation and automation platform, directly into your AI workflow. Manage your document templates, generate new PDF or Word files from JSON data, and track your generated output using natural language.

### What you can do

- **Template Oversight** — List and retrieve detailed information and field schemas for all your document templates.
- **Document Generation** — Trigger the document generation engine to create new files instantly using provided data fields.
- **Output Tracking** — Monitor generated documents, including their current status and secure download URLs.
- **Field Intelligence** — Identify exactly which data points are required to populate specific templates accurately.

### How it works

1. Connect the Docdown integration to your AI assistant.
2. Authorize using your Docdown API Key (found in your account settings).
3. Orchestrate your document automation and reporting through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly generate contracts or reports from structured data on the go.
- **Admin Teams** — Monitor document generation status and access output files via chat.
- **Developers** — Audit template schemas and test document generation logic instantly.


## Available Tools
- **generate_new_document**: Generate a new document using a specific template and data object
- **get_docdown_account_metadata**: Retrieve metadata and usage limits for your Docdown account
- **get_document_status**: Get the current status and download URL for a specific document
- **get_template_field_schema**: Identify exactly which fields are required to populate a template
- **get_template_details**: Get detailed information and field schema for a specific template
- **list_published_templates**: Identify templates that are currently in a "Published" status
- **list_generated_documents**: List all documents that have been generated from templates
- **list_recently_generated_docs**: Identify documents that have been generated in the last 24 hours
- **list_doc_templates**: List all available document templates in your Docdown account
- **search_templates_by_name**: Search for a document template using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docdown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available document templates."

**🤖 AI Agent:**
> I've found 5 templates in your account, including 'Service Agreement v2', 'Monthly Performance Report', and 'Customer Invoice'. Would you like to see the required fields for the Service Agreement?

---

**👤 You:**
> "Generate a new 'Customer Invoice' with data: {'name': 'John Doe', 'amount': 150}."

**🤖 AI Agent:**
> I've triggered the generation for 'Customer Invoice'. The document is currently being processed. I will provide the download URL as soon as it is ready. The document ID is 'DOC-12345'.

---

**👤 You:**
> "Show me the status of document 'DOC-12345'."

**🤖 AI Agent:**
> Document 'DOC-12345' is now 'Completed'. You can download it here: [https://api.docdown.io/download/...] (Link expires in 24 hours). Should I list other recently generated documents?


## ❓ FAQ

**Q: How do I get a Docdown API Key?**
Log in to your Docdown account, navigate to the API section in your settings, and you can generate or retrieve your unique API Key from there.

**Q: Which document formats are supported?**
Docdown primarily supports generating high-quality PDF and Microsoft Word (.docx) files from your templates and data.

**Q: Can the agent show me the required fields for a template?**
Yes, you can use the get_template_field_schema tool to retrieve exactly which data keys and types are needed to populate a specific template.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docdown](https://vinkius.com/mcp/docdown)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Docdown** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `docdown` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Docdown** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docdown": {
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
