# Azure Blob Container MCP Server

This MCP does exactly one thing: it manages files in a single Azure Blob Container. That's its only function, and nothing else. Incredible for giving your AI secure file storage.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-blob-container)

## Overview
**Category:** industry-titans
**Tools Count:** 4

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


## Installation & Usage

To install and use the **Azure Blob Container** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-blob-container](https://vinkius.com/mcp/azure-blob-container)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
