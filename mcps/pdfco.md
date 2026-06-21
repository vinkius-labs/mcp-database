# PDF.co MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pdfco)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pdfco-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pdfco-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Parse, generate, merge, and convert PDF documents programmatically with an API that handles complex document processing tasks.

## Description
Connect your **PDF.co** account to any AI agent and take full control of your document orchestration and data extraction through natural conversation. PDF.co provides a professional-grade suite of tools for PDF manipulation, allowing you to convert files to various formats, perform high-fidelity OCR on scanned images, and manage document security directly from your chat interface.

### What you can do

- **Document Conversion Orchestration** — Convert PDFs and images to plain text, JSON, CSV, or XML programmatically to ensure your data pipelines are always synchronized.
- **High-Fidelity OCR Intelligence** — Perform high-resolution OCR on scanned documents and handwritten text directly from the AI interface to extract critical metadata.
- **Data Extraction & Merging** — Extract tables and metadata or merge multiple PDF files via natural language to maintain a high-fidelity document repository.
- **Security & Protection Control** — Add or remove password protection and manage PDF security settings using simple AI commands.
- **Operational Monitoring** — Track background job statuses and manage account balance to ensure your document production is always optimized.

### How it works

1. Subscribe to this server
2. Enter your PDF.co API Key from your dashboard settings
3. Start managing your document processing from Claude, Cursor, or any MCP-compatible client

No more manual data entry from scanned invoices. Your AI acts as a dedicated document analyst or data processing coordinator.

### Who is this for?

- **Data Analysts & Accountants** — quickly extract tabular data from PDF reports and monitor financial records without switching apps.
- **Operations Managers** — automate the merging and splitting of logistics documents via natural conversation.
- **Developers** — integrate real-time PDF conversion and OCR capabilities directly within the chat.


## Available Tools
- **check_job_status**: Check async job status
- **pdf_to_csv**: Convert PDF tables to CSV
- **pdf_to_json**: Convert PDF to structured JSON
- **pdf_to_text**: Convert PDF to plain text
- **pdf_to_xml**: Convert PDF to XML
- **extract_pdf_meta**: Extract PDF metadata with AI
- **get_account_info**: co account and credit balance.

Get account information
- **merge_pdfs**: Merge multiple PDFs
- **ocr_image**: Perform OCR on an image
- **protect_pdf**: Add password to PDF
- **split_pdf**: Split a PDF
- **unprotect_pdf**: Remove password from PDF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PDF.co** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the PDF at 'https://example.com/invoice.pdf' to structured JSON."

**🤖 AI Agent:**
> I've processed the document. I have the structured JSON data containing all text and layout metadata. Would you like me to summarize the financial totals?

---

**👤 You:**
> "Convert the uploaded invoice PDF into a structured JSON with all line items extracted."

**🤖 AI Agent:**
> Invoice parsed successfully. Vendor: Acme Supplies Ltd. Invoice #INV-2025-0847. Date: May 8, 2025. 4 line items extracted: Widget A ($125 x 10), Widget B ($89 x 5), Service Fee ($250 x 1), Shipping ($45 x 1). Subtotal: $2,040. Tax (8%): $163.20. Total: $2,203.20. Payment terms: NET30. All fields extracted with 98% confidence.

---

**👤 You:**
> "Merge these 3 quarterly report PDFs into a single document and add page numbers."

**🤖 AI Agent:**
> 3 PDFs merged successfully into a single document (42 pages total). Q1 Report (14 pages), Q2 Report (16 pages), and Q3 Report (12 pages) combined in order. Sequential page numbers added in the footer. Output file size: 2.8 MB. Download link generated and valid for 24 hours.


## Installation & Usage

To install and use the **PDF.co** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdfco](https://vinkius.com/mcp/pdfco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
