# PDFMonkey MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pdfmonkey)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate dynamic PDF documents from JSON data and HTML templates with an API built for high-volume document automation.

## Description
Connect your **PDFMonkey** account to any AI agent and take full control of your document automation and PDF orchestration through natural conversation. PDFMonkey provides a high-fidelity rendering engine that transforms HTML and CSS templates into professional-grade PDF files using dynamic payloads.

### What you can do

- **Document & PDF Orchestration** — Generate professional documents like invoices, shipping labels, or certificates programmatically by injecting dynamic JSON into your HTML templates.
- **Template Lifecycle Management** — List all managed templates and retrieve detailed metadata to ensure your document designs are always synchronized.
- **Generation Intelligence** — Access and monitor your document generation history and retrieve secure, temporary download links directly from the AI interface.
- **Status & Workflow Control** — Track document generation statuses (pending, generated) via natural language to ensure your automated pipelines are always optimized.
- **Operational Monitoring** — Track system responses and manage document records using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your PDFMonkey Secret Key from your account settings
3. Start generating and managing your PDFs from Claude, Cursor, or any MCP-compatible client

No more manual status checking or searching for download links. Your AI acts as a dedicated document automation coordinator or production lead.

### Who is this for?

- **Finance Teams** — quickly generate automated invoices and financial reports without switching apps.
- **Operations Managers** — automate the creation of logistics documents and monitor generation history via natural conversation.
- **Developers** — integrate real-time PDF generation and template management directly within the chat.


## Available Tools (11)
- **generate_pdf**: Generation is asynchronous.

Generate a new PDF from a template
- **delete_generated_pdf**: Delete a generated document
- **get_pdf_details**: Get details and download link for a PDF
- **check_pdf_status**: Quickly check generation status
- **get_template**: Get details for a template
- **get_workspace**: Get details for a specific workspace
- **list_generated_documents**: List recently generated PDFs
- **list_templates**: List all PDF templates
- **list_workspaces**: List all workspaces
- **regenerate_document**: Regenerate a PDF document
- **update_document**: Update an existing PDF document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PDFMonkey** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a document using template 'tpl_abc123' with this data: {'name': 'John Doe', 'amount': 150}."

**🤖 AI Agent:**
> I've initiated the document generation. The status is currently 'pending' (ID: doc_xyz). Would you like me to check when the download link is ready?

---

**👤 You:**
> "Generate a batch of 50 personalized certificate PDFs from my training completion template."

**🤖 AI Agent:**
> Batch generation started for 50 certificates using template "Training Certificate v2" (tpl_4821). Status: Processing. 12 of 50 completed so far. Each certificate includes the participant's name, course title, completion date, and a unique certificate number. Estimated completion: 4 minutes. You will be notified when all documents are ready for download.

---

**👤 You:**
> "Show me the current status and preview of document doc_9234 generated yesterday."

**🤖 AI Agent:**
> Document doc_9234 status: Success. Template: "Monthly Report". Generated: May 12, 2025 at 3:45 PM. File size: 847 KB (6 pages). The document includes 3 charts, 2 tables, and a cover page. Download URL is active and expires in 72 hours. Last viewed: today at 9:15 AM.


## ❓ FAQ

**Q: Can my AI automatically find the download link for a document after it has been generated?**
Yes! Use the `get_document` tool with the Document ID. Your agent will respond with complete metadata, including the `download_url` if the status is 'success'. Note that these links are temporary for security.

**Q: How do I find my PDFMonkey Secret Key?**
Log in to your PDFMonkey dashboard, navigate to **My Account**, and you will find your unique secret API key in the 'Secret Key' section.

**Q: What status should I expect when a document is first created?**
The initial status is usually 'pending' while the document is being rendered. You can ask the AI to poll the status until it becomes 'success' to retrieve the download link.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdfmonkey](https://vinkius.com/mcp/pdfmonkey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PDFMonkey** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pdfmonkey` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PDFMonkey** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pdfmonkey": {
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
