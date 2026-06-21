# Html2Pdf MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html2pdf)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/html2pdf-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/html2pdf-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert any website URL or raw HTML into high-quality PDF documents directly from your AI agent.

## Description
Transform web content and raw HTML into professional PDF files with **Html2Pdf**. This server allows your AI agent to generate documents, reports, and invoices on the fly with full control over layout, styling, and security.

### What you can do

- **URL to PDF** — Provide any public URL to capture a pixel-perfect PDF snapshot of the webpage.
- **HTML Rendering** — Send raw HTML strings to generate custom documents like invoices, certificates, or resumes.
- **Layout Customization** — Control page format (A4, Letter, etc.), orientation (landscape), and precise margins for a perfect print.
- **Advanced Styling** — Use `waitFor` for JavaScript execution and `media` types (print/screen) for accurate CSS rendering.
- **Security & Permissions** — Protect your documents with user/owner passwords and restrict actions like printing or copying.
- **Async Callbacks** — Handle large document generation via webhooks for seamless background processing.

### How it works

1. Subscribe to this server
2. Enter your Html2Pdf API Key
3. Start generating documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate document generation workflows without setting up complex headless browser clusters.
- **Business Analysts** — Quickly turn web-based reports or dashboards into shareable PDF files.
- **Content Creators** — Archive web articles or format HTML content into clean, portable documents.


## Available Tools
- **generate_pdf**: Returns the PDF as a base64 encoded string, or triggers an async callback if callBackUrl is provided.

Convert HTML or a URL to a PDF document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Html2Pdf** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert https://google.com to a PDF in A4 format and landscape orientation."

**🤖 AI Agent:**
> I've initiated the PDF generation for Google.com with landscape orientation. The document is being processed and will be returned as a base64 encoded string.

---

**👤 You:**
> "Generate a PDF from this HTML code: '<h1>Invoice #123</h1><p>Total: $50</p>' and name the file 'invoice.pdf'."

**🤖 AI Agent:**
> Processing your HTML invoice... I've generated the PDF with the filename 'invoice.pdf'. You can now access the document payload.

---

**👤 You:**
> "Create a password-protected PDF of https://example.com using 'secret123' as the password."

**🤖 AI Agent:**
> Securing your document... I've generated a password-protected PDF for the requested URL. The file is encrypted and will require 'secret123' to be opened.


## Installation & Usage

To install and use the **Html2Pdf** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html2pdf](https://vinkius.com/mcp/html2pdf)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
