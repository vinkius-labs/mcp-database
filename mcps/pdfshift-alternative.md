# PDFShift MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pdfshift-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert URLs or HTML to PDF and images — manage templates, track credits, and automate document generation via high-performance API.

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


## Available Tools (15)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PDFShift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert https://news.ycombinator.com to a PDF in landscape orientation."

**🤖 AI Agent:**
> I've initiated the conversion for Hacker News. The PDF has been generated in landscape mode. [Download Link/Binary Data]

---

**👤 You:**
> "List all my saved HTML templates and show the credits I have left."

**🤖 AI Agent:**
> You have 3 templates: 'invoice-v1', 'report-monthly', and 'welcome-email'. Your current balance is 450 credits.

---

**👤 You:**
> "Show me the logs for my last 5 conversion attempts."

**🤖 AI Agent:**
> Fetching your recent logs... Here are the last 5 conversions, including status codes, source URLs, and processing times.


## ❓ FAQ

**Q: Can I test the conversion without spending my credits?**
Yes. Use the `sandbox` parameter set to `true` in tools like `convert_to_pdf`. This generates a watermarked document for development purposes at no credit cost.

**Q: How do I generate a document using a saved template?**
First, ensure your template is created using `create_template`. Then, use `generate_from_template` providing the template slug and the dynamic data you want to inject.

**Q: Can I capture a full-page screenshot as an image?**
Absolutely. Use `convert_to_png`, `convert_to_jpeg`, or `convert_to_webp` and set the `fullpage` parameter to `true` to capture the entire scrollable area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pdfshift-alternative](https://vinkius.com/mcp/pdfshift-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PDFShift** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pdfshift-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PDFShift** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pdfshift-alternative": {
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
