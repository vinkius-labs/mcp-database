# Docamatic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docamatic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate professional PDFs from templates with dynamic data injection for invoices, reports, and custom documents at scale.

## Description
Connect your **Docamatic** account to any AI agent and take full control of your document automation and media production workflows through natural conversation.

### What you can do

- **Document Orchestration** — Convert raw HTML strings or live website URLs into professional, high-fidelity PDF and image files programmatically
- **Template Intelligence** — Create invoices, packing slips, and certificates by injecting dynamic data into predefined built-in templates directly through your agent
- **PDF Manipulation** — Draw new elements (text, QR codes, images) onto existing PDF documents or merge multiple files into a single finalized document
- **Visual Intelligence** — Capture high-quality full-page screenshots of any live website with automatic JavaScript rendering handling
- **Workflow Monitoring** — Access your complete directory of recently generated documents and monitor your production history directly from your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Docamatic account settings
3. Start generating and modifying professional documents from Claude, Cursor, or any MCP client

No more manual document formatting or complex rendering pipelines. Your AI acts as your dedicated document engineer and media production coordinator.

### Who is this for?

- **Finance & Admin Teams** — instantly generate professional invoices and reports using natural language commands
- **Developers & Ops** — automate the creation of technical documentation and capture website snapshots without leaving your terminal
- **Marketing Professionals** — scale the production of dynamic certificates and visual collateral through simple AI queries


## Available Tools (8)
- **generate_image_from_html**: Convert HTML or URL to Image
- **generate_pdf_from_template**: g. invoice1, packing_slip1) with JSON data.

Generate a PDF from a predefined template
- **list_generation_history**: List recently generated documents
- **list_available_builtin_templates**: List common document templates
- **merge_multiple_pdfs**: Combine several PDF files into one
- **take_web_screenshot**: Handles rendering automatically.

Capture a full-page website screenshot
- **add_elements_to_pdf**: Draw text or images onto an existing PDF
- **generate_pdf_from_html**: Convert HTML or URL to PDF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docamatic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a professional PDF of the website 'https://vinkius.com'."

**🤖 AI Agent:**
> Document rendering triggered! I'm converting 'https://vinkius.com' into a high-fidelity PDF. You can download the finalized file here: [download_url]. Need me to capture a screenshot as well?

---

**👤 You:**
> "Create an invoice for 'Acme Corp' using the 'invoice3' template."

**🤖 AI Agent:**
> Invoice generated! I've populated the 'invoice3' template with your data for Acme Corp. The document is now ready. Would you like to merge it with any past project reports?

---

**👤 You:**
> "Take a full-page screenshot of 'https://news.google.com'."

**🤖 AI Agent:**
> Visual captured! I've taken a high-quality full-page screenshot of the specified news URL. You can view the image here: [image_url]. Shall I check your recent generation history for other files?


## ❓ FAQ

**Q: How do I find my Docamatic API Key?**
Log in to your account and navigate to the **API Key** section in your settings to generate or copy your unique access token.

**Q: Can I use my own custom HTML strings?**
Yes! The `generate_pdf_from_html` and `generate_image_from_html` tools accept raw HTML strings as source input.

**Q: Does it support merging existing PDF files?**
Absolutely. Use the `merge_multiple_pdfs` tool and provide an array of public URLs to combine them into a single PDF document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docamatic](https://vinkius.com/mcp/docamatic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Docamatic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `docamatic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Docamatic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docamatic": {
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
