# Azure Blob Container MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-blob-container)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/azure-blob-container-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/azure-blob-container-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it manages files in a single Azure Blob Container. That's its only function, and nothing else. Incredible for giving your AI secure file storage.

## Description
This server strips away dangerous global Azure permissions. It gives your AI agent one surgical superpower: **the ability to read, write, and list files inside one specific Blob Container.**

By strictly scoping access, your AI can safely persist data, analyze documents, and manage its own workload without ever touching your critical cloud infrastructure.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single container. It cannot list other containers or delete your company's production backups.
- **Native Azure Integration:** Direct, high-performance interactions with Azure Blob Storage using Entra ID Service Principals.
- **Plug & Play File System:** Instantly gives your agent a massive cloud hard drive to store its memories, generated assets, and processed reports.


## Available Tools
- **delete_blob**: Use with caution.

Delete a file from the configured container
- **get_blob**: Download and read the contents of a specific file
- **list_blobs**: You can optionally provide a prefix to filter by a specific "folder" path.

List files (blobs) inside the configured Azure Blob Container
- **put_blob**: Create or overwrite a file in the configured container


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Azure Blob Container** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all files in the 'invoices/' folder."

**🤖 AI Agent:**
> I found 3 files with the prefix 'invoices/': invoice_001.json, invoice_002.json, and invoice_003.json.

---

**👤 You:**
> "Read the contents of 'config.json'."

**🤖 AI Agent:**
> Here is the content of 'config.json': `{"retentionDays": 30, "active": true}`.

---

**👤 You:**
> "Save this summary as 'reports/summary.txt'."

**🤖 AI Agent:**
> The file 'reports/summary.txt' has been created successfully in the Azure Blob Container.


## Installation & Usage

To install and use the **Azure Blob Container** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-blob-container](https://vinkius.com/mcp/azure-blob-container)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
