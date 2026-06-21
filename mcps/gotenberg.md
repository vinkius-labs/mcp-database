# Gotenberg MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gotenberg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gotenberg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gotenberg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Convert URLs, HTML, and Markdown to PDF or screenshots, and manage PDF files with tools for merging, splitting, and metadata editing.

## Description
Connect your **Gotenberg** instance to any AI agent to handle complex document conversions and PDF manipulations through natural language. Gotenberg provides a developer-friendly API for converting various document formats into PDF and images.

### What you can do

- **Web to PDF/Image** — Convert live URLs, raw HTML, or Markdown into high-quality PDF documents or screenshots using Chromium.
- **Office Conversion** — Transform Office documents (docx, xlsx, pptx) into PDF format via LibreOffice integration.
- **PDF Manipulation** — Merge multiple PDFs into a single file or split existing documents into separate pages.
- **Metadata & Bookmarks** — Read and write PDF metadata, manage bookmarks, and embed attachments directly into your documents.
- **Flexible Rendering** — Customize paper size, margins, orientation, and wait for specific JS expressions before rendering.

### How it works

1. Subscribe to this server
2. Enter your Gotenberg instance URL (and optional credentials)
3. Start generating and modifying documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — automate the generation of invoices, reports, or documentation directly from code or templates.
- **Content Creators** — quickly turn Markdown notes or web content into polished PDF files.
- **Operations Teams** — streamline document workflows by merging reports and managing PDF metadata without manual tools.


## Available Tools
- **convert_html_to_pdf**: Returns the base64 encoded PDF.

Convert raw HTML to PDF using Chromium
- **convert_office_to_pdf**: ) to PDF using the downloadFrom parameter.

Convert Office documents to PDF using LibreOffice
- **convert_markdown_to_pdf**: Convert Markdown to PDF using Chromium
- **convert_url_to_pdf**: Returns the base64 encoded PDF.

Convert a URL to PDF using Chromium
- **embed_pdf_attachments**: Embed attachments into a PDF
- **get_health**: Get Gotenberg health status
- **merge_pdfs**: Merge multiple PDFs into one
- **read_pdf_bookmarks**: Read bookmarks from a PDF
- **read_pdf_metadata**: Read metadata from a PDF
- **screenshot_html**: Take a screenshot of raw HTML
- **screenshot_markdown**: Take a screenshot of Markdown
- **screenshot_url**: Returns the base64 encoded image.

Take a screenshot of a URL
- **split_pdf**: Returns a ZIP file containing the split PDFs.

Split a PDF into multiple files
- **get_version**: Get Gotenberg version
- **write_pdf_bookmarks**: Write bookmarks to a PDF
- **write_pdf_metadata**: Write metadata to a PDF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gotenberg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert https://gotenberg.dev to a PDF in landscape orientation."

**🤖 AI Agent:**
> I've converted the URL to a landscape PDF. You can download the generated document now.

---

**👤 You:**
> "Take a PNG screenshot of this HTML: '<h1>Hello MCP</h1>'"

**🤖 AI Agent:**
> I've generated a PNG screenshot of your HTML content. Here is the image.

---

**👤 You:**
> "Read the metadata of the PDF I just uploaded."

**🤖 AI Agent:**
> Accessing metadata... The PDF was created by 'Gotenberg' on 2023-10-27, with the title 'Project Report'.


## Installation & Usage

To install and use the **Gotenberg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gotenberg](https://vinkius.com/mcp/gotenberg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
