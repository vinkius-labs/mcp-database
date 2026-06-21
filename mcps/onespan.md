# OneSpan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onespan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Automate e-signature workflows via OneSpan Sign — create transaction packages, upload documents, and manage signing statuses directly from any AI agent.

## Description
Connect your **OneSpan Sign** account to any AI agent to streamline your digital transaction management and document signing workflows through natural conversation.

### What you can do

- **Transaction Packages** — Create new signing packages to organize documents and signers for any business deal.
- **Document Management** — Upload documents directly to existing packages with specific metadata and content configurations.
- **Workflow Control** — Update package statuses (e.g., moving a package to 'SENT') to trigger the signing process for all participants.
- **Bulk Retrieval** — Download all signed documents from a completed package as a single ZIP file for easy archiving.
- **Event Notifications** — Configure callback settings to receive real-time updates on events like package completion or signer activity.

### How it works

1. Subscribe to this server
2. Enter your OneSpan API Key (and optionally your Base URL)
3. Start managing your e-signature workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal & Compliance Teams** — quickly initiate signing processes and verify document statuses without manual portal navigation.
- **Sales Operations** — automate the creation of contract packages and track real-time progress of client signatures.
- **HR Professionals** — manage onboarding documents and employee agreements efficiently through AI-driven commands.


## Available Tools
- **configure_callback**: Configure or receive event notifications
- **create_package**: Create a new transaction package
- **download_documents_zip**: Download all signed documents in a zip file
- **update_package**: g., to SENT).

Update package status
- **upload_document**: Upload a document to a package


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneSpan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new OneSpan transaction package for 'Service Agreement 2024'."

**🤖 AI Agent:**
> I've initiated the package creation. The new transaction 'Service Agreement 2024' has been created with Package ID: `pkg-99283`. You can now start uploading documents to it.

---

**👤 You:**
> "Upload the document metadata for package ID 'pkg-99283'."

**🤖 AI Agent:**
> The document metadata has been successfully uploaded to package `pkg-99283`. The document is now registered and ready for signer placement.

---

**👤 You:**
> "Update the status of package 'pkg-99283' to SENT."

**🤖 AI Agent:**
> Package `pkg-99283` has been updated to SENT. OneSpan Sign is now notifying the signers to review and sign the documents.


## ❓ FAQ

**Q: How do I finalize and send a package to signers?**
Use the `update_package` tool with the target Package ID and a payload setting the status to 'SENT'. This triggers the notification emails to all designated signers.

**Q: Can I download all signed documents from a package at once?**
Yes! The `download_documents_zip` query allows you to retrieve a single ZIP file containing every signed document associated with a specific Package ID.

**Q: How do I set up automated notifications for completed transactions?**
You can use the `configure_callback` action to define a URL and events (like 'PACKAGE_COMPLETE') that OneSpan should notify when they occur.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onespan](https://vinkius.com/mcp/onespan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OneSpan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `onespan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneSpan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onespan": {
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
