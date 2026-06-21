# PDFShift MCP Server

Convert URLs or HTML to PDF and images — manage templates, track credits, and automate document generation via high-performance API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pdfshift-alternative)

## Overview
**Category:** productivity
**Tools Count:** 15

## Description
Connect **PDFShift** to your AI agent to transform web content into professional documents. This server provides a direct bridge to a high-performance conversion engine capable of handling complex CSS, JavaScript, and modern web layouts.

### What you can do

- **Multi-Format Conversion** — Convert any URL or HTML string into PDF, PNG, JPEG, or WebP formats using `convert_to_pdf`, `convert_to_png`, and more.
- **Template System** — Store and manage reusable HTML templates with `create_template` and `generate_from_template` for dynamic document generation.
- **Granular Control** — Customize margins, headers, footers, viewports, and orientation for pixel-perfect results.
- **Account Management** — Monitor your usage with `get_credits_usage`, inspect `list_logs`, and manage billing via `list_invoices`.
- **Cloud & Webhooks** — Export files directly to S3/Google Storage or receive results asynchronously via webhooks.

### How it works

1. Subscribe to this server
2. Enter your PDFShift API Key
3. Start generating documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate invoices, receipts, and reports without maintaining a local headless browser.
- **Content Teams** — Archive web pages or generate social media preview images instantly.
- **Operations** — Convert internal HTML dashboards into shareable PDF reports for stakeholders.


## Available Tools
- **convert_to_jpeg**: Convert URL or HTML to JPEG
- **convert_to_pdf**: Use filename parameter to get a JSON response with an S3 URL instead of raw binary.

Convert URL or HTML to PDF
- **convert_to_png**: Convert URL or HTML to PNG
- **convert_to_webp**: Convert URL or HTML to WEBP
- **create_template**: Create a new template
- **delete_template**: Delete a template
- **generate_from_template**: Generate document from a template
- **get_account**: Get account details
- **get_credits_usage**: Get credits usage
- **get_log**: Get log by request ID
- **get_template_html**: Get template HTML content
- **list_invoices**: List invoices
- **list_logs**: List recent logs
- **list_templates**: List all templates
- **update_template**: Update an existing template


## Installation & Usage

To install and use the **PDFShift** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdfshift-alternative](https://vinkius.com/mcp/pdfshift-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
