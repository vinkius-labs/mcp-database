# Affinda MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/affinda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Intelligent document processing — parse resumes, invoices, and IDs via AI.

## Description
Connect your **Affinda** account to your AI agent to unlock powerful intelligent document processing (IDP). From automatically extracting details from resumes and invoices to auditing document statuses across your workspaces, your agent handles structured data extraction through natural conversation.

### What you can do

- **Automated Document Parsing** — Upload PDFs or images of resumes, invoices, and passports for high-accuracy JSON extraction
- **Workspace Oversight** — List and audit documents within your specific workspaces to maintain organizational control
- **Extraction Model Management** — List available document types (Resume, Invoice, Receipt, etc.) supported by your account
- **Real-time Status Tracking** — Retrieve the parsing status and technical metadata for any uploaded document
- **Metadata Insights** — Quickly identify processing errors or missing data across your document library directly from chat

### How it works

1. Subscribe to this server
2. Enter your Affinda Bearer Token
3. Start parsing documents and managing your workspaces through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruitment Teams** — automate resume screening and extract candidate metadata effortlessly
- **Accounts Payable** — audit invoice data extraction and verify payment details via AI
- **Operations Managers** — monitor document processing workflows and manage workspace settings
- **Compliance Officers** — retrieve parsed identity documents for risk assessment and verification


## Available Tools (5)
- **list_documents**: Retrieve all parsed documents in an Affinda workspace with their processing status
- **get_document**: Retrieve the fully structured JSON data and status for a specific processed document in Affinda
- **create_document**: Defaults to synchronous waiting for the output.

Upload and parse a PDF or image into Affinda via its public URL for high-accuracy JSON extraction
- **list_workspaces**: Retrieve all container workspaces for documents created within your Affinda account
- **list_document_types**: Retrieve exactly which parsing models the Affinda account supports (e.g. Resume, Invoice, Passport)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Affinda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all documents in my 'HR Recruitment' workspace."

**🤖 AI Agent:**
> I've retrieved the documents from the 'HR Recruitment' workspace. You have 15 resumes currently processed. Would you like to see the extracted contact details for the latest candidates?

---

**👤 You:**
> "Parse this resume URL: https://example.com/cv.pdf using the 'resume' model."

**🤖 AI Agent:**
> I've started the parsing process for the resume. The document identifier is 'abc-123'. I'll wait for the synchronous extraction to complete... Done! I have the structured data for John Doe, including his 5 years of experience in Python development.

---

**👤 You:**
> "List the available document types in my account."

**🤖 AI Agent:**
> I've retrieved your supported document models. You can currently parse Resumes, Invoices, Receipts, and Passports. Would you like to see the specific fields extracted by the Invoice model?


## ❓ FAQ

**Q: How do I find my Affinda API Key?**
Log in to Affinda, click on your profile avatar, and go to **Settings** > **API Keys**. You can generate a new token there. Remember to copy it immediately, as it is only shown once.

**Q: What document types are supported?**
Affinda supports dozens of specialized models including Resumes, Invoices, Receipts, Passports, Driver Licenses, and Purchase Orders. Use the `list_document_types` tool to see the full list for your account.

**Q: Can I parse a document via a public URL?**
Yes! The `create_document` tool accepts a `url` parameter. Simply provide the direct link to the PDF or image, and Affinda will retrieve and parse it automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/affinda](https://vinkius.com/mcp/affinda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Affinda** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `affinda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Affinda** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "affinda": {
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
