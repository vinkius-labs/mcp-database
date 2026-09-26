# Household Identity Document Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-identity-document-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A privacy-conscious system for indexing and retrieving household identity documents and metadata.

## Description
This MCP server provides a secure way to manage and retrieve identity document metadata within a household. It allows AI agents to perform specific tasks such as using `get_document_by_holder` to find documents for a specific person, `check_document_validity` to verify if a document is still valid, `locate_document_access` to find storage locations, and `search_expired_documents` to identify documents that need renewal.


## Available Tools (4)
- **check_document_validity**: Checks if a specific document is currently valid based on its issuance and expiry dates
- **get_document_by_holder**: Provide householdId to narrow the search to a specific household.

Retrieves all indexed identity documents belonging to a specific person
- **locate_document_access**: Identifies where a document is stored and who can be contacted to access it
- **search_expired_documents**: Identifies all documents within a household that have passed their expiry date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Identity Document Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What documents does John Doe have in his household?"

**🤖 AI Agent:**
> John Doe has a Passport and a Driver's License indexed in the system.

---

**👤 You:**
> "Is the passport with ID 12345 still valid?"

**🤖 AI Agent:**
> Yes, the passport is valid until December 31, 2028.

---

**👤 You:**
> "List all expired documents for household HH-987."

**🤖 AI Agent:**
> The expired documents for household HH-987 are a Birth Certificate (expired 2023-01-15) and a Driver's License (expired 2022-05-20).


## ❓ FAQ

**Q: How does this server protect privacy?**
The server uses privacy-conscious indexing, returning only the minimum necessary metadata required to locate or identify a document without exposing sensitive biometric or full-document data.

**Q: Can I check if a passport is expired?**
Yes, you can use the `check_document_validity` tool to verify the status of a specific document based on its expiry date.

**Q: How do I find where a document is stored?**
You can use the `locate_document_access` tool to identify the storage location and the primary contact for a specific document type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-identity-document-index](https://vinkius.com/en/ai-agent-connect/household-identity-document-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Identity Document Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-identity-document-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Identity Document Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-identity-document-index": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
