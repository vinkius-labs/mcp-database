# DocsGenFlow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docsgenflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create documents automatically from templates with merge fields that pull data from your systems and generate polished output.

## Description
Connect your **DocsGenFlow** account to any AI agent and take full control of your document generation orchestration and automated file creation through natural conversation.

### What you can do

- **Template Portfolio Orchestration** — List and manage your entire portfolio of document templates (PDF, DOCX) programmatically, retrieving detailed merge fields
- **Document Creation Intelligence** — Programmatically trigger and monitor document generation jobs using custom JSON data inputs
- **Workflow Architecture Monitoring** — Access real-time status updates for automated document flows and track individual file processing directly through your agent
- **Metadata Management** — Programmatically retrieve hosted file URLs and generation IDs to maintain a perfectly coordinated digital archive
- **Operational Monitoring** — Verify account-level API connectivity and monitor document orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your DocsGenFlow dashboard (Settings > API)
3. Start orchestrating your document growth from Claude, Cursor, or any MCP client

No more manual filling of templates or missing document generation errors. Your AI acts as your dedicated document coordinator and flow architect.

### Who is this for?

- **Operations Managers** — instantly trigger document batches and monitor generation status using natural language commands
- **Legal & Compliance Leads** — verify individual document metadata and track creation history without leaving your creative workspace
- **Developers** — integrate high-speed DocsGenFlow document data into custom CRM and ERP pipelines through simple AI queries


## Available Tools (10)
- **check_docsgenflow_status**: Verify DocsGenFlow API connectivity
- **create_template**: Create a template
- **download_document**: Download a document
- **generate_document**: Pass data as JSON with field-value pairs.

Generate a document
- **get_account**: Get account info
- **get_document**: Get document details
- **get_template**: Get template details
- **list_documents**: List generated documents
- **list_history**: List generation history
- **list_templates**: List all templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocsGenFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all document templates in my DocsGenFlow account."

**🤖 AI Agent:**
> I've retrieved your templates. You currently have 10 active profiles, including 'Invoicing Template' and 'Sales Contract'. Would you like the detailed merge field metadata for any of them?

---

**👤 You:**
> "Check the status of the last 5 document generation jobs."

**🤖 AI Agent:**
> Job intelligence orchestrated! For your recent requests, I've identified 5 document generation jobs. 4 are 'COMPLETED' and 1 is 'PROCESSING'. I've retrieved the generation metadata for your review. Need help retrieving the final file URLs?

---

**👤 You:**
> "Show my DocsGenFlow document generation metrics for this month."

**🤖 AI Agent:**
> Operational monitoring orchestrated! This month, your account has processed 1,000 document generation requests, with a 99% success rate. Your API connection is healthy. Shall I retrieve the detailed template usage breakdown?


## ❓ FAQ

**Q: How do I find my DocsGenFlow API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I retrieve generation status via AI?**
Yes! The `list_history` tool allows your agent to retrieve status metadata for all your document generation requests.

**Q: How do I list my document templates?**
Use the `list_templates` tool to retrieve your complete directory along with the unique identifiers for all managed assets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docsgenflow](https://vinkius.com/mcp/docsgenflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DocsGenFlow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `docsgenflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DocsGenFlow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docsgenflow": {
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
