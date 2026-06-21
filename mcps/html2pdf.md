# Html2Pdf MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/html2pdf)
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


## ❓ FAQ

**Q: Can I wait for JavaScript to finish before generating the PDF?**
Yes! Use the `waitFor` parameter (up to 10 seconds) in the `generate_pdf` tool. This is ideal for pages that rely on async data loading or animations before they are ready to be captured.

**Q: Is it possible to add custom headers and footers to the document?**
Absolutely. You can provide HTML strings for `headerTemplate` and `footerTemplate` to include page numbers, logos, or dates on every page of your generated PDF.

**Q: Can I protect the generated PDF with a password?**
Yes. By setting the `userPassword` parameter, the server will trigger AES 128-bit encryption, requiring that password to open the document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/html2pdf](https://vinkius.com/mcp/html2pdf)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Html2Pdf** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `html2pdf` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Html2Pdf** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "html2pdf": {
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
