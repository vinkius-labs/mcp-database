# PDF Munk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pdf-munk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate PDF and image generation via PDF Munk — convert HTML/URL to PDF, merge documents, and compress files directly from any AI agent.

## Description
Connect your **PDF Munk** account to any AI agent and simplify your document generation, file manipulation, and visual asset orchestration through natural conversation.

### What you can do

- **PDF Generation** — Convert raw HTML or public website URLs into high-quality PDF documents for invoices, reports, and more
- **Image Creation** — Generate PNG/JPG screenshots and social cards from any web page URL programmatically
- **Document Manipulation** — Merge multiple PDF files into one or compress existing PDFs to optimize storage and sharing
- **Visual Feedback** — Receive hosted URLs or base64 strings for every generated asset directly through your agent
- **Direct Control** — Power your document workflows and content pipeline without leaving your conversation

### How it works

1. Subscribe to this server
2. Enter your PDF Munk API Key from your dashboard
3. Start generating professional documents from Claude, Cursor, or any MCP-compatible client


## Available Tools (12)
- **add_watermark**: Add watermark
- **check_pdfmunk_status**: Verify connectivity
- **compress_pdf**: Compress PDF
- **generate_pdf_from_html**: Generate PDF from HTML
- **generate_pdf_from_template**: Generate from template
- **generate_pdf_from_url**: Generate PDF from URL
- **generate_image**: Generate image
- **generate_screenshot**: Capture screenshot
- **get_template**: Get template details
- **list_templates**: List templates
- **merge_pdfs**: Merge PDFs
- **split_pdf**: Split PDF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PDF Munk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 'https://google.com' to a PDF document."

**🤖 AI Agent:**
> I've generated the PDF for you. You can download it here: [PDF Link].

---

**👤 You:**
> "Generate a shipping label PDF for order #ORD-4521 with customs declaration data."

**🤖 AI Agent:**
> Shipping label PDF generated for order #ORD-4521. Destination: Munich, Germany. Weight: 2.3 kg. Customs declaration included with HS codes for 3 items. Carrier: DHL Express. Tracking barcode embedded. The label includes sender and recipient addresses, package dimensions, and a return label on page 2. File ready for printing at 4x6 inches.

---

**👤 You:**
> "Convert my HTML report template into a paginated PDF with headers and footers."

**🤖 AI Agent:**
> HTML to PDF conversion complete. Output: 18 pages. Page size: A4. Custom header applied with company logo and report title on each page. Footer includes page numbers ("Page X of 18") and generation timestamp. Table of contents auto-generated on page 1. All CSS styles preserved including charts and data tables. File size: 1.2 MB.


## ❓ FAQ

**Q: Can I convert a website URL to a PDF using my AI agent?**
Yes! Use the `convert_url_to_pdf` tool and provide the target URL. Your agent will return a link to the generated PDF document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdf-munk](https://vinkius.com/mcp/pdf-munk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PDF Munk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pdf-munk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PDF Munk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pdf-munk": {
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
