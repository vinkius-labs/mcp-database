# Archbee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/archbee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage documentation spaces, sync OpenAPI specs, and organize technical knowledge directly from your AI agent.

## Description
Connect **Archbee** to your AI agent to streamline your technical documentation and knowledge management workflows. This server allows you to interact with your Archbee organization using natural language.

### What you can do

- **Document Management** — Create, update, retrieve, and delete documents using Markdown. Search across your entire organization instantly.
- **OpenAPI Synchronization** — Sync your API definitions (JSON/YAML) to specific document trees and enable features like 'Try It' or custom backends.
- **Space & Organization** — Create, clone, update, and publish documentation spaces. Organize them into groups for better structure.
- **Content Import** — Quickly import Markdown content into your documentation structure.
- **Global Search** — Query your entire knowledge base to find specific technical details or guides.

### How it works

1. Subscribe to this server
2. Enter your Archbee API Key
3. Start managing your technical docs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Sync OpenAPI specs and update technical docs without leaving the IDE.
- **Product Managers** — Search through product requirements and documentation spaces to answer questions quickly.
- **Technical Writers** — Manage document lifecycles and publish updates to different environments seamlessly.


## Available Tools (19)
- **create_space**: Create a new documentation space
- **create_update_doc**: Create a new document or update an existing one
- **delete_doc**: Delete a specific document
- **delete_space_group**: Remove a space group
- **delete_space**: Permanently remove a space
- **discard_suggestion**: Discard a suggested change
- **get_display_rules**: Retrieve the display rules configured for the organization
- **export_organization**: Export the entire organization data
- **get_doc**: Retrieve the content of a specific document
- **import_content**: Import Markdown content into a document
- **info_openapi**: Retrieve information about a synchronized OpenAPI document
- **merge_suggestion**: Merge a suggested change document into the primary document
- **publish_space**: Publish a space to a specific environment
- **search_docs**: Search for documents within your organization
- **sync_openapi**: Synchronize an OpenAPI definition with an Archbee document
- **update_space**: Update the settings or metadata of a space
- **upload_file**: Upload a file to Archbee storage
- **clone_space**: Create a duplicate of an existing space
- **create_space_group**: Organize spaces into a new group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Archbee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my Archbee docs for 'authentication flow'."

**🤖 AI Agent:**
> I found 3 documents related to 'authentication flow'. The most relevant is 'OAuth2 Implementation Guide' (ID: abc123...). Would you like me to retrieve its content?

---

**👤 You:**
> "Sync this OpenAPI YAML content to document tree 21charIDhere."

**🤖 AI Agent:**
> Starting OpenAPI synchronization... The API definition has been successfully synced to the document tree. The 'Try It' feature is enabled as requested.

---

**👤 You:**
> "Create a new document in Archbee with the title 'Onboarding' and content '# Welcome...'"

**🤖 AI Agent:**
> I've created the 'Onboarding' document. You can access it or update it further using the ID: doc_xyz789.


## ❓ FAQ

**Q: Can I synchronize my Swagger or OpenAPI files to Archbee using this server?**
Yes! Use the `sync_openapi` tool. You can provide the file content and the target document tree ID to automatically update your API documentation.

**Q: How do I search for a specific topic across all my documents?**
Use the `search_docs` tool with your search query. The AI will return a list of relevant documents found within your Archbee organization.

**Q: Is it possible to publish a documentation space to a live environment?**
Absolutely. Use the `publish_space` tool and specify the target environment to make your documentation updates live.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/archbee](https://vinkius.com/mcp/archbee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Archbee** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `archbee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Archbee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "archbee": {
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
