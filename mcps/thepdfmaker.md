# ThePDFMaker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thepdfmaker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Transform HTML templates into pixel-perfect PDF documents with an API designed for invoices, reports, and branded output.

## Description
Connect your **PDFMaker** account to any AI agent and take full control of your document automation and PDF orchestration through natural conversation. PDFMaker provides a powerful and flexible platform for transforming structured JSON data into professional-grade PDF files using templates from Google Docs, MS Word, or its native editor.

### What you can do

- **Document & PDF Orchestration** — Generate high-quality documents like invoices, certificates, or reports programmatically by merging dynamic data into your templates.
- **Template Lifecycle Management** — List all managed templates and retrieve detailed placeholder metadata directly from the AI interface to ensure your mapping is always synchronized.
- **Generation Intelligence** — Access and monitor your PDF generation history and retrieve direct download links for final documents via natural language.
- **Webhook & Automation Control** — Create and manage webhooks to ensure your document workflows are always optimized using simple AI commands.
- **Operational Monitoring** — Track account credits, usage stats, and system health to ensure your production is always high-performing.

### How it works

1. Subscribe to this server
2. Enter your PDFMaker API Key (Bearer Token) from your dashboard
3. Start generating and managing your professional documents from Claude, Cursor, or any MCP client

No more manual editing in document processors for repetitive tasks. Your AI acts as a dedicated document manager or production coordinator.

### Who is this for?

- **Operations Managers** — quickly retrieve document statuses and monitor generation history without switching apps.
- **Finance Teams** — automate the creation of invoices and reports via natural conversation.
- **Developers** — integrate real-time document generation and credit tracking directly within the chat.


## Available Tools (12)
- **create_webhook**: Add new notification
- **delete_pdf_template**: Remove a template
- **generate_pdf**: Create PDF from template
- **get_credit_balance**: Check API credits
- **get_pdf_status**: Get document link
- **get_user_profile**: Get account info
- **get_api_status**: Check connectivity
- **get_template_details**: Get template info
- **list_asset_files**: List uploaded assets
- **list_recent_pdfs**: List recent generations
- **list_pdf_templates**: List all templates
- **list_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThePDFMaker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my PDF templates in PDFMaker."

**🤖 AI Agent:**
> I've retrieved your templates. You have 3 active designs including 'Invoice Template v2' and 'Monthly Report'. Which one would you like to use for generation?

---

**👤 You:**
> "Generate a professional invoice PDF using my corporate template for client Meridian Corp."

**🤖 AI Agent:**
> Invoice PDF generated successfully using template "Corporate Invoice v3". Client: Meridian Corp. Invoice #2025-0523. 3 line items totaling $8,750. Payment terms: NET15. The PDF includes your company logo, footer with bank details, and a QR code for direct payment. File size: 124 KB. Ready for download or email delivery.

---

**👤 You:**
> "List all available PDF templates in my account and when they were last modified."

**🤖 AI Agent:**
> You have 8 templates. "Corporate Invoice v3" was last modified on May 1st and is your most used template (234 generations). "Sales Quote" modified April 28th (89 uses). "NDA Template" updated April 15th (45 uses). "Certificate of Completion" from March 20th (67 uses). 4 additional templates available with combined 123 generations.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific template by its ID?**
Yes! Use the `get_template` tool with the Template ID. Your agent will respond with complete metadata for the model, including all available placeholder fields in seconds.

**Q: How do I find my PDFMaker API Key?**
Log in to your PDFMaker account, navigate to **Settings** > **API Key**, and you will find your unique secret token there.

**Q: What document formats does PDFMaker support for templates?**
PDFMaker supports a variety of sources including native HTML templates, MS Word (.docx), and Google Docs, allowing you to choose the best editor for your needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thepdfmaker](https://vinkius.com/mcp/thepdfmaker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ThePDFMaker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thepdfmaker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ThePDFMaker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thepdfmaker": {
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
