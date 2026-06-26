# Paperless-ngx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/paperless-ngx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your digital archive via Paperless-ngx — search documents, upload files, manage tags, and organize correspondents directly from any AI agent.

## Description
Connect your **Paperless-ngx** instance to any AI agent and transform your document archive into a searchable, conversational knowledge base.

### What you can do

- **Document Discovery** — Use `list_documents` with full-text search or filter by tags and dates to find exactly what you need in seconds.
- **File Operations** — Upload new documents with `upload_document`, download originals with `download_document`, or get instant visual context with `preview_document` and `thumb_document`.
- **Metadata Management** — Organize your library by creating and updating tags, correspondents, and document types using dedicated tools like `create_tag` or `update_correspondent`.
- **Deep Inspection** — Fetch complete OCR text and metadata for any specific file using `get_document` to help your AI analyze contents.
- **Saved Views** — Access your predefined filters and organizational structures with `list_saved_views`.

### How it works

1. Subscribe to this server
2. Provide your Paperless-ngx API URL and Personal API Token
3. Start chatting with your documents in Claude, Cursor, or any MCP-compatible client

No more manual searching through folders. Your AI acts as a digital librarian that knows every word in your archive.

### Who is this for?

- **Home Office Users** — instantly find utility bills, tax records, or manuals without digging through physical or digital piles.
- **Legal & Admin Teams** — query specific correspondents or document types to build reports or verify information quickly.
- **Researchers** — manage large collections of PDFs and papers with automated tagging and content retrieval.


## Available Tools (26)
- **list_tags**: List all tags
- **delete_tag**: Delete a tag
- **download_document**: Download the actual document file
- **get_correspondent**: Retrieve correspondent details
- **get_document**: Retrieve details of a specific document
- **get_document_type**: Retrieve document type details
- **get_tag**: Retrieve tag details
- **list_correspondents**: List all correspondents
- **list_document_types**: List all document types
- **list_documents**: Supports filtering and searching via query parameters.

List all documents in Paperless-ngx
- **preview_document**: Get a preview of the document
- **thumb_document**: Get the document thumbnail
- **update_correspondent**: Update a correspondent
- **update_document**: Update document metadata
- **update_document_type**: Update a document type
- **update_tag**: Update a tag
- **upload_document**: Upload a new document
- **create_tag**: Create a new tag
- **create_correspondent**: Create a new correspondent
- **create_document_type**: Create a new document type
- **create_saved_view**: Create a new saved view
- **list_saved_views**: List all saved views
- **delete_correspondent**: Delete a correspondent
- **delete_document**: Delete a document
- **delete_document_type**: Delete a document type
- **delete_saved_view**: Delete a saved view


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paperless-ngx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all documents related to 'Electricity Bill' from 2023."

**🤖 AI Agent:**
> I've searched your archive using `list_documents`. I found 3 documents: 'Jan 2023 Electricity' (ID: 101), 'Feb 2023 Electricity' (ID: 105), and 'March 2023 Electricity' (ID: 110). Would you like to see the details of one of them?

---

**👤 You:**
> "Upload a new document titled 'Contract 2024' with tag ID 12."

**🤖 AI Agent:**
> Processing the upload... I've successfully used `upload_document` to add 'Contract 2024'. It has been assigned ID 250 and is now being processed by Paperless-ngx for OCR.

---

**👤 You:**
> "Get the full content and a preview of document ID 42."

**🤖 AI Agent:**
> I've retrieved the data for document 42 using `get_document` and `preview_document`. The document is a 'Lease Agreement'. The OCR text mentions a monthly rent of $1,200. I've also generated a preview link for you.


## ❓ FAQ

**Q: Can I search for documents using specific tags or date ranges?**
Yes. The `list_documents` tool allows you to filter by `tags__id__in` and `created__date__gte`. You can also perform a full-text search using the `query` parameter.

**Q: Is it possible to see a preview of a document without downloading the whole file?**
Absolutely. Use the `preview_document` or `thumb_document` tools to get visual representations of the document content directly through the agent.

**Q: Can I create new organization categories like tags or correspondents via AI?**
Yes, you have full management capabilities. You can use `create_tag`, `create_correspondent`, and `create_document_type` to organize your archive on the fly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperless-ngx](https://vinkius.com/mcp/paperless-ngx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paperless-ngx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paperless-ngx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paperless-ngx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paperless-ngx": {
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
