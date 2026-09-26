# Estate Document Location Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/estate-document-location-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A centralized indexing service for locating and managing sensitive estate-related documentation.

## Description
This MCP server provides a centralized indexing service to help users locate and manage sensitive estate-related documentation. It connects AI agents to a structured repository of record categories, storage locations, and authorized access contacts. Using tools like `get_document_by_category` and `find_location_by_document`, agents can quickly identify where specific files are kept and who to contact for retrieval. The service also includes `list_all_access_contacts` to identify authorized individuals and `verify_location_freshness` to ensure the information remains reliable and up to date.


## Available Tools (4)
- **get_document_by_category**: Answers the question: Where can I find documents belonging to a specific classification?
- **list_all_access_contacts**: Answers the question: Who are the people I can reach out to regarding estate matters?
- **verify_location_freshness**: Answers the question: Is the information for this location still reliable and up to date?
- **find_location_by_document**: Answers the question: I have a specific document name; where is it located and who do I contact?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Estate Document Location Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where can I find documents belonging to the Vital Records category?"

**🤖 AI Agent:**
> The Vital Records include the Birth Certificate (located in the Digital Vault) and the Marriage License (located in the Safe Deposit Box).

---

**👤 You:**
> "I have the 'Last Will and Testament'. Where is it located and who is the contact?"

**🤖 AI Agent:**
> The Last Will and Testament is located in the Legal Filing Cabinet. Please contact the Executor, Jane Doe, for retrieval.

---

**👤 You:**
> "Who are the authorized contacts for Financial Assets?"

**🤖 AI Agent:**
> The authorized contacts for Financial Assets are John Smith (Trustee) and Sarah Jenkins (Executor).


## ❓ FAQ

**Q: How can I find all documents in a specific category?**
You can use the `get_document_by_category` tool by providing the specific classification name you are looking for.

**Q: How do I know if the location information is still accurate?**
The `verify_location_freshness` tool allows you to check if the location or contact information for a specific document is still current.

**Q: Who can I contact to access a specific document?**
You can use `find_location_by_document` to find the specific access contact for a document, or `list_all_access_contacts` to see a list of authorized individuals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/estate-document-location-guide](https://vinkius.com/en/ai-agent-connect/estate-document-location-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Estate Document Location Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `estate-document-location-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Estate Document Location Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "estate-document-location-guide": {
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
