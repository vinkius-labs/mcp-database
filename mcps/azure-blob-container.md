# Azure Blob Container MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/azure-blob-container)
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


## ❓ FAQ

**Q: Why limit the agent to a single Blob Container?**
To enforce zero-trust security. An autonomous AI agent should not have the ability to read or delete files across your entire Azure Storage Account. By scoping it to a single container, you eliminate the risk of accidental or malicious data loss in other containers.

**Q: How does authentication work?**
It uses Microsoft Entra ID (formerly Azure AD). You provide a Service Principal's Tenant ID, Client ID, and Client Secret. The MCP engine automatically handles the OAuth 2.0 token exchange securely.

**Q: Can I read binary files like images?**
The current engine is optimized for text and JSON-based workflows. Reading large binary files directly into the LLM's context window is not recommended.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/azure-blob-container](https://vinkius.com/mcp/azure-blob-container)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Azure Blob Container** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `azure-blob-container` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Azure Blob Container** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "azure-blob-container": {
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
