# DocRaptor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docraptor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert HTML to professional PDFs and Excel spreadsheets using the high-quality Prince XML engine.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocRaptor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a test PDF document from the URL https://example.com and make it hosted."

**🤖 AI Agent:**
> I've initiated the document creation. Since it's a test, it will have a watermark. You can download your hosted PDF here: https://docraptor.com/download/example-link

---

**👤 You:**
> "Check the status of my async document with ID 'status_12345'."

**🤖 AI Agent:**
> The document generation is complete! It resulted in a 3-page PDF. You can download it using the provided URL.

---

**👤 You:**
> "List the last 5 documents generated in my account."

**🤖 AI Agent:**
> I've retrieved your recent documents. Here are the last 5: 'Invoice_Jan.pdf', 'Report_Q4.xlsx', 'Test_Layout.pdf', etc. Would you like details on any of these?


## ❓ FAQ

**Q: Can I generate a test document without using my document balance?**
Yes! When calling the `create_document` tool, set the `test` parameter to `true`. This creates a free, watermarked document for testing your layout.

**Q: How do I handle very large HTML files that take a long time to render?**
Use the `async` parameter in `create_document`. The tool will return a `status_id`, which you can then use with `get_document_status` to check when the file is ready for download.

**Q: Can I get a direct URL to share the generated document?**
Yes, by setting the `hosted` parameter to `true` in the `create_document` tool. DocRaptor will host the file and return a `download_url` that you can share.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docraptor](https://vinkius.com/mcp/docraptor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DocRaptor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `docraptor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DocRaptor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docraptor": {
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
