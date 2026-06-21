# PSPDFKit (Nutrient) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pspdfkit-nutrient)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pspdfkit-nutrient-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pspdfkit-nutrient-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Professional PDF and document processing — generate, convert, OCR, and edit documents via the Nutrient API.

## Description
Connect **PSPDFKit (Nutrient)** to your AI agent and handle complex document workflows through natural conversation. This server provides high-performance tools for document generation, transformation, and accessibility.

### What you can do

- **PDF Generation** — Convert raw HTML content into professional PDF documents instantly using the `generate_pdf` tool.
- **OCR & Searchability** — Extract text from images or scanned PDFs using `ocr_document` to make them searchable and readable by your agent.
- **Format Conversion** — Transform Office files (DOCX, PPTX) and images into standardized PDFs with `convert_to_pdf`.
- **Advanced Building** — Apply complex operations like redaction, watermarking, and document merging via the `build_document` action.
- **Accessibility Compliance** — Automatically tag PDFs for PDF/UA compliance using `autotag_pdf` to ensure accessibility standards.
- **Web Viewing** — Prepare documents for web integration by creating viewer sessions and uploading files to the Viewer API.

### How it works

1. Subscribe to this server
2. Enter your Nutrient (PSPDFKit) API Key
3. Start processing documents directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Automate document generation and conversion pipelines without leaving the IDE.
- **Legal & Compliance Teams** — Quickly redact sensitive information and ensure PDF accessibility.
- **Operations Managers** — Streamline document workflows by converting legacy files and scanned images into searchable assets.


## Available Tools
- **autotag_pdf**: Auto-tag a PDF for accessibility (PDF/UA)
- **build_document**: Advanced document processing (redact, watermark, etc)
- **convert_to_pdf**: ) to PDF.

Convert Office or Image files to PDF
- **create_viewer_session**: Generate a session token for the Viewer API
- **generate_pdf**: Generate a PDF from HTML content
- **ocr_document**: Perform OCR on an image or PDF
- **upload_viewer_document**: Upload a document to the Viewer API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PSPDFKit (Nutrient)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a PDF from this HTML: '<h1>Invoice #123</h1><p>Amount: $50.00</p>'"

**🤖 AI Agent:**
> I've generated the PDF from your HTML content. You can access the document here: [URL].

---

**👤 You:**
> "Convert this Word document to PDF: https://example.com/report.docx"

**🤖 AI Agent:**
> Processing the conversion... The DOCX file has been successfully converted to PDF. Here is your file: [URL].

---

**👤 You:**
> "Run OCR on this scanned image to make it searchable: https://example.com/scan.jpg"

**🤖 AI Agent:**
> I've performed OCR on the image. The text has been extracted and the document is now searchable. You can download it here: [URL].


## Installation & Usage

To install and use the **PSPDFKit (Nutrient)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pspdfkit-nutrient](https://vinkius.com/mcp/pspdfkit-nutrient)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
