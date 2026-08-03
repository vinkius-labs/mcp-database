# Ugosign MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ugosign)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Sign documents electronically with a platform that supports advanced electronic signatures and complies with European regulations.

## Description
Connect your **Ugosign** account to any AI agent to streamline your electronic signature and document approval workflows. Ugosign provides a powerful REST API for programmatically managing signature requests, tracking document statuses, and maintaining a secure audit trail of all signed agreements.

### What you can do

- **Signature Request Orchestration** — List and create new electronic signature requests for one or more recipients with detailed tracking
- **Document Lifecycle Tracking** — Monitor the real-time status of your documents and signature requests from draft to fully executed
- **Audit Trail Monitoring** — Access detailed metadata for all signature requests to maintain a secure and compliant record of your agreements
- **Organization Intelligence** — Retrieve detailed information about your Ugosign organization to maintain an overview of your team's signing capacity
- **Frictionless Approvals** — Get a comprehensive overview of active signature requests and pending actions using natural language commands

### How it works

1. Subscribe to this server
2. Enter your Ugosign API Key from your developer portal
3. Start managing your electronic signatures from Claude, Cursor, or any MCP client

### Who is this for?

- **Legal & Compliance Teams** — monitor agreement statuses and manage audit trails more efficiently using natural language
- **Sales Operations** — automate the creation of signature requests for contracts and order forms
- **Developers** — integrate real-time electronic signature intelligence into custom business and legal dashboards


## Available Tools (6)
- **create_signature_request**: Pass data as a JSON string.

Create a new signature request
- **get_document**: Get document details
- **get_organization**: Get organization details
- **get_signature_request**: Get signature request details
- **list_documents**: List all documents
- **list_signature_requests**: List all signature requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ugosign** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active signature requests in Ugosign."

**🤖 AI Agent:**
> I've retrieved your signature requests. You have 5 active requests, including 'Employment Agreement - John Doe' (Pending) and 'Sales Contract - Acme Corp' (Viewed).

---

**👤 You:**
> "What is the status of signature request 'req_123'?"

**🤖 AI Agent:**
> Signature request 'req_123' ('Service Agreement') is currently 'Signed' by all parties. The execution was completed today at 10:15 AM.

---

**👤 You:**
> "Show me the details for my Ugosign organization."

**🤖 AI Agent:**
> I've retrieved your organization details. Your account is 'Vinkius Legal' (ID: 552) and you have unlimited signature requests remaining on your current plan.


## ❓ FAQ

**Q: How do I get my Ugosign API Key?**
Log in to your Ugosign account, navigate to the **Developer API** or **Integrations** section, and copy your secret Bearer Token.

**Q: Can I track the status of a specific signature request?**
Yes, use the `get_signature_request` tool with the unique ID to see if it is 'pending', 'viewed', or 'signed'.

**Q: Does it support multiple recipients?**
Absolutely. You can specify one or more recipients when creating a new signature request via the `create_signature_request` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ugosign](https://vinkius.com/mcp/ugosign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ugosign** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ugosign` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ugosign** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ugosign": {
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
