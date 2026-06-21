# Pdfcrowd MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pdfcrowd)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert HTML, web pages, and documents to PDF or images. Generate invoices and extract text from PDFs directly via AI.

## Description
Transform web content and documents with the **Pdfcrowd** MCP server. This powerful integration allows your AI agent to convert HTML to high-quality PDFs or images, extract text from existing PDFs, and generate professional business documents like invoices from raw data.

### What you can do

- **Web to PDF/Image** — Convert any URL or raw HTML string into a polished PDF or image (PNG, JPG, WebP, GIF) using `convert_html_to_pdf` and `convert_html_to_image`.
- **Document Conversion** — Transform PDF documents back into HTML or plain text for easy analysis and data extraction using `convert_pdf_to_html` and `convert_pdf_to_text`.
- **Business Automation** — Generate professional invoices and receipts directly from JSON data using pre-built templates with `generate_business_document`.
- **Fine-grained Control** — Customize page sizes, orientation, margins, and viewports for pixel-perfect results.

### How it works

1. Subscribe to this server
2. Enter your Pdfcrowd Username and API Key
3. Start converting documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate report generation and web archiving directly from the IDE.
- **Finance Teams** — Instantly generate invoices and receipts from structured data.
- **Content Managers** — Convert web pages to static documents for documentation and sharing.


## Available Tools
- **convert_html_to_image**: Returns base64 encoded image data.

Capture a screenshot of a web page or HTML content
- **convert_html_to_pdf**: Returns base64 encoded PDF data.

Convert a web page or HTML string to PDF
- **convert_pdf_to_html**: Returns base64 encoded HTML data.

Transform a PDF document into HTML
- **convert_pdf_to_text**: Returns base64 encoded text data.

Transform a PDF document into plain text
- **generate_business_document**: Returns base64 encoded PDF data.

Generate professional documents (invoices, receipts) from JSON data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pdfcrowd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the web page https://example.com to a PDF in landscape orientation."

**🤖 AI Agent:**
> I've initiated the conversion for https://example.com. I've set the orientation to landscape as requested. Your PDF is ready for download.

---

**👤 You:**
> "Take a PNG screenshot of https://news.ycombinator.com with a width of 1280px."

**🤖 AI Agent:**
> Capturing the screenshot... I've generated a PNG image of Hacker News at a 1280px viewport width. You can view the image now.

---

**👤 You:**
> "Generate a modern invoice for $1200 USD for 'Software Consulting' with 1 item."

**🤖 AI Agent:**
> I'm generating your modern invoice. I've added 'Software Consulting' as the line item for a total of $1200 USD. The PDF document has been created.


## ❓ FAQ

**Q: Can I convert a raw HTML string instead of a URL?**
Yes! Use the `convert_html_to_pdf` or `convert_html_to_image` tools and provide your HTML code in the `text` parameter instead of using the `url` parameter.

**Q: How do I generate a professional invoice from my data?**
Use the `generate_business_document` tool. Provide the `document_type` as 'invoice', and include your line items, total, and currency in the JSON payload to get a styled PDF.

**Q: Is it possible to extract plain text from a PDF file?**
Absolutely. Use the `convert_pdf_to_text` tool with the URL of your PDF. You can also enable `no_layout` if you want the text in reading order without layout preservation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdfcrowd](https://vinkius.com/mcp/pdfcrowd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pdfcrowd** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pdfcrowd` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pdfcrowd** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pdfcrowd": {
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
