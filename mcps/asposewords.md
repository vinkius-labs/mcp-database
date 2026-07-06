# Aspose.Words MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/asposewords)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate, convert, and manipulate Word documents programmatically with enterprise-grade document processing capabilities.

## Description
Connect your **Aspose.Words Cloud** account to any AI agent and take full control of your professional document lifecycle and content manipulation workflows through natural conversation.

### What you can do

- **Multimodal Document Conversion** — Programmatically convert base64-encoded files across 40+ formats (DOCX, PDF, HTML, Markdown, etc.) with high-fidelity formatting preservation
- **Content Orchestration** — Perform advanced search-and-replace, insert watermarks, and accept all tracked changes to coordinate document revisions in real-time
- **Document Intelligence** — Extract high-fidelity statistics including word counts and page metrics, or render specific pages into image formats (PNG, JPEG) for instant previews
- **Security & Protection** — Programmatically apply password protection or restrict editing to maintain high-fidelity document integrity and compliance
- **Storage Architecture** — Manage your directory of cloud-hosted files and oversee document lifecycle from upload to deletion directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **JWT Token** from the Aspose Cloud Dashboard (My Apps > Client ID/Secret)
3. Start localizing and processing your document assets from Claude, Cursor, or any MCP client

No more manual toggling between Word editors or slow desktop conversion tools. Your AI acts as your dedicated document engineer and formatting coordinator.

### Who is this for?

- **Legal & Compliance Teams** — instantly apply watermarks and accept revisions using natural language commands
- **Administrative Staff** — automate high-volume document conversions and content replacements without leaving your workspace
- **Developers** — integrate high-speed cloud-based document manipulation into custom business workflows through simple AI queries


## Available Tools (10)
- **accept_all_revisions**: Accept track changes
- **add_watermark**: Insert a watermark
- **delete_cloud_file**: Delete a document
- **get_document_statistics**: Get document statistics
- **list_cloud_files**: List files in storage
- **protect_document**: Protect document
- **convert_document**: Convert document format
- **render_document_page**: Render specific page
- **replace_text_in_document**: Replace text
- **split_document**: Split document into pages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aspose.Words** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in my Aspose Cloud root storage."

**🤖 AI Agent:**
> I've retrieved your cloud files. You currently have 5 documents, including 'Proposal_v1.docx' (ID: 1024) and 'Contract.pdf'. Which one should we process or convert?

---

**👤 You:**
> "Convert 'Proposal_v1.docx' to PDF and add a 'DRAFT' watermark."

**🤖 AI Agent:**
> Document processing initiated! I've started the high-fidelity conversion to PDF and added the 'DRAFT' watermark. I'll provide the secure download link as soon as the render is complete.

---

**👤 You:**
> "Render page 1 of 'Contract.pdf' as a PNG image."

**🤖 AI Agent:**
> Page rendering triggered! I'm converting the first page of your contract into a high-fidelity PNG image. This is useful for instant previews in your agent. Need help with other pages?


## ❓ FAQ

**Q: How do I find my Aspose JWT Token?**
Log in to the [**Aspose Cloud Dashboard**](https://dashboard.aspose.cloud/), go to **My Apps**, create or select an app, and generate a JWT token using your Client ID and Client Secret.

**Q: Can I replace text inside a Word file via AI?**
Yes! The `replace_text_in_document` tool allows your agent to find and update specific strings within documents hosted in your Aspose Cloud storage.

**Q: How do I check document page count?**
Use the `get_document_statistics` tool to retrieve word count, page count, and other high-fidelity structural metadata directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/asposewords](https://vinkius.com/mcp/asposewords)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aspose.Words** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `asposewords` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aspose.Words** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "asposewords": {
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
