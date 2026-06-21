# Stirling PDF MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stirling-pdf)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage PDF documents via Stirling PDF — add watermarks, convert images to PDF, sign documents with certificates, and monitor server metrics directly.

## Description
Connect your **Stirling PDF** instance to any AI agent and take full control of your document workflows through natural conversation. This server allows you to process PDF files, convert formats, and monitor your self-hosted infrastructure.

### What you can do

- **Document Manipulation** — Add text watermarks with custom opacity and font sizes, or convert images directly into PDF documents.
- **Digital Security** — Sign PDF documents using certificates with specific reasons and location metadata.
- **Server Monitoring** — Track application status, version info, and detailed request metrics (POST/GET) across all endpoints.
- **Advanced Operations** — Use the generic tool runner to access specialized features like merging, splitting, or extracting images from PDFs.
- **Enterprise Metrics** — Access Prometheus metrics for deep observability into your document processing pipeline.

### How it works

1. Subscribe to this server
2. Enter your Stirling PDF Base URL and API Key
3. Start processing documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate PDF processing tasks directly from your IDE or terminal.
- **System Administrators** — Monitor the health and load of your Stirling PDF instance in real-time.
- **Legal & Admin Teams** — Quickly sign or watermark documents without leaving your AI chat interface.


## Available Tools
- **add_watermark**: Add a watermark to a PDF document
- **cert_sign**: Sign a PDF document with a certificate
- **get_all_requests**: Get POST requests count for all endpoints
- **get_all_unique_requests**: Get unique users count for all endpoints
- **get_load**: Get total count of GET requests
- **get_prometheus_metrics**: Get Prometheus metrics (requires Enterprise tier)
- **get_requests**: Get total count of POST requests
- **get_status**: Get application status and version information
- **get_unique_requests**: Get count of unique users for POST requests
- **img_to_pdf**: Convert an image to a PDF document
- **run_generic_tool**: Pass additional parameters as a JSON string.

Run any Stirling PDF tool by its ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stirling PDF** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the current status and version of my Stirling PDF server."

**🤖 AI Agent:**
> I've checked your instance. It is currently online running version 0.25.1. All systems are operational.

---

**👤 You:**
> "Add a 'CONFIDENTIAL' watermark to this PDF with 0.5 opacity."

**🤖 AI Agent:**
> Processing the document... I've applied the 'CONFIDENTIAL' text watermark with the requested settings. You can now download the processed PDF.

---

**👤 You:**
> "Convert this image to a PDF document named 'report.pdf'."

**🤖 AI Agent:**
> Converting image... I have successfully generated 'report.pdf' from your image file using the maintainAspectRatio fit option.


## ❓ FAQ

**Q: Can I add a text watermark to a PDF document using this server?**
Yes! Use the `add_watermark` tool. You can specify the text, font size, and opacity to apply a professional watermark to any PDF file provided in base64 format.

**Q: How do I monitor the traffic and load on my Stirling PDF instance?**
You can use `get_requests` to see POST counts, `get_load` for GET requests, or `get_prometheus_metrics` if you are on the Enterprise tier for detailed observability.

**Q: Is it possible to perform other operations like merging or splitting PDFs?**
Yes, the `run_generic_tool` action allows you to execute any Stirling PDF tool by its ID (e.g., 'merge-pdfs' or 'split-pages') by passing the required parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stirling-pdf](https://vinkius.com/mcp/stirling-pdf)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stirling PDF** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stirling-pdf` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stirling PDF** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stirling-pdf": {
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
