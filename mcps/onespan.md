# OneSpan MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onespan)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/onespan-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/onespan-mcp)
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


## Installation & Usage

To install and use the **OneSpan** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onespan](https://vinkius.com/mcp/onespan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
