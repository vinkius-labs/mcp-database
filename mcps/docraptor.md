# DocRaptor MCP Server

Convert HTML to professional PDFs and Excel spreadsheets using the high-quality Prince XML engine.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docraptor)

## Overview
**Category:** productivity
**Tools Count:** 4

## Description
Connect **DocRaptor** to your AI agent to transform HTML content or URLs into professional-grade PDFs and Excel documents. Powered by the Prince XML engine, it provides the most accurate CSS-to-PDF rendering available.

### What you can do

- **Document Creation** — Generate PDFs, XLS, or XLSX files directly from HTML strings or public URLs using `create_document`.
- **Asynchronous Processing** — Handle large documents in the background by setting the async flag and monitoring progress with `get_document_status`.
- **Hosted Documents** — Create publicly accessible, temporary download links for your generated files without managing your own storage.
- **Advanced Styling** — Leverage full Prince XML support for headers, footers, page numbers, and complex CSS layouts.
- **Management & Security** — List previously generated documents and retrieve DocRaptor's IP addresses for secure asset fetching.

### How it works

1. Subscribe to this server
2. Enter your DocRaptor API Key
3. Start generating high-fidelity documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate the creation of invoices, reports, and certificates directly from your coding environment.
- **Data Analysts** — Export complex data visualizations or tables into perfectly formatted Excel spreadsheets.
- **Operations Teams** — Convert web-based dashboards or internal tools into shareable PDF reports with a single prompt.


## Available Tools
- **create_document**: Use async=true or hosted=true to avoid large binary responses in the tool output.

Create a PDF or Excel document from HTML
- **get_document_status**: Check the status of an asynchronous document generation
- **list_documents**: List previously generated documents
- **list_ips**: List IP addresses used by DocRaptor


## Installation & Usage

To install and use the **DocRaptor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docraptor](https://vinkius.com/mcp/docraptor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
