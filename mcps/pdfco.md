# PDF.co MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pdfco)
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


## ❓ FAQ

**Q: Can my AI automatically find and extract a specific table from a PDF?**
Yes! Use the `convert_to_csv` or `convert_to_json` tools. Your agent will respond with the structured tabular data from the document in seconds, ready for analysis.

**Q: How do I find my PDF.co API Key?**
Log in to your PDF.co account, navigate to the main dashboard, and you will find your unique secret API key (starting with your email reference or key string) there.

**Q: Does this support handwritten text recognition?**
Absolutely. PDF.co's high-fidelity OCR engine is designed to handle both printed and handwritten text with high accuracy across multiple languages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdfco](https://vinkius.com/mcp/pdfco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PDF.co** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pdfco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PDF.co** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pdfco": {
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
