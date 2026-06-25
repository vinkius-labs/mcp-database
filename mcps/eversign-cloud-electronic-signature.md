# Eversign (Cloud Electronic Signature) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eversign-cloud-electronic-signature)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage electronic signatures via Eversign — list businesses, create documents, and handle templates directly from any AI agent.

## Description
Connect your **Eversign** account to any AI agent to streamline your document signing workflows through natural conversation.

### What you can do

- **Business Management** — List all businesses associated with your account to retrieve the necessary Business IDs for operations.
- **Document Creation** — Generate new documents for signature from scratch, including custom files, signers, and specific fields.
- **Template Automation** — Create reusable templates or generate new signing requests from existing template hashes instantly.
- **Sandbox Testing** — Use the sandbox mode to test your document workflows without creating legally binding contracts.
- **Embedded Signing** — Create drafts specifically configured for iFrame or embedded signing environments.

### How it works

1. Subscribe to this server
2. Enter your Eversign API Access Key
3. Start managing your digital contracts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & HR Teams** — quickly send out NDAs, offer letters, or contracts without leaving your workspace
- **Sales Operations** — automate the generation of sales agreements from templates directly from your CRM context
- **Developers** — test e-signature integrations using the sandbox mode and inspect business structures via API


## Available Tools (2)
- **list_businesses**: Use this to find the business_id required for document operations.

List all businesses associated with your account
- **create_document**: Can also be used to create reusable templates or generate documents from templates.

Create a new document, create a template, or use an existing template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eversign (Cloud Electronic Signature)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all businesses in my Eversign account."

**🤖 AI Agent:**
> I've retrieved your business profiles. You have access to 'Global Logistics Ltd' (ID: 54321) and 'Creative Agency' (ID: 98765). Which business ID would you like to use for your document?

---

**👤 You:**
> "Create a test document in sandbox mode for business 54321 with a signer named Alice."

**🤖 AI Agent:**
> I've initiated the document creation in sandbox mode for business 54321. The document has been prepared for Alice. Since this is sandbox mode, it will not be legally binding.

---

**👤 You:**
> "Generate a document from template 'abc123hash' for business 98765."

**🤖 AI Agent:**
> Processing template 'abc123hash'... I have successfully generated a new document for business 98765 based on your template. Would you like to check the status of the signers?


## ❓ FAQ

**Q: How do I find the Business ID required for creating documents?**
You can use the `list_businesses` tool. It will return a list of all businesses associated with your account along with their unique IDs.

**Q: Can I test document creation without it being legally binding?**
Yes! When using the `create_document` tool, set the `sandbox` parameter to true. This allows you to test the workflow with a testing prefix.

**Q: Is it possible to generate a document from an existing template?**
Absolutely. Use the `create_document` tool and provide the `template_id` (the hash of your template) to generate a document based on that template.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eversign-cloud-electronic-signature](https://vinkius.com/mcp/eversign-cloud-electronic-signature)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Eversign (Cloud Electronic Signature)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eversign-cloud-electronic-signature` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Eversign (Cloud Electronic Signature)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eversign-cloud-electronic-signature": {
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
