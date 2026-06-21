# Paperless-ngx MCP Server

Manage your digital archive via Paperless-ngx — search documents, upload files, manage tags, and organize correspondents directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/paperless-ngx)

## Overview
**Category:** loved-by-devs
**Tools Count:** 26

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


## Available Tools
- **create_correspondent**: Create a new correspondent
- **create_document_type**: Create a new document type
- **create_saved_view**: Create a new saved view
- **create_tag**: Create a new tag
- **delete_correspondent**: Delete a correspondent
- **delete_document**: Delete a document
- **delete_document_type**: Delete a document type
- **delete_saved_view**: Delete a saved view
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
- **list_saved_views**: List all saved views
- **list_tags**: List all tags
- **preview_document**: Get a preview of the document
- **thumb_document**: Get the document thumbnail
- **update_correspondent**: Update a correspondent
- **update_document**: Update document metadata
- **update_document_type**: Update a document type
- **update_tag**: Update a tag
- **upload_document**: Upload a new document


## Installation & Usage

To install and use the **Paperless-ngx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/paperless-ngx](https://vinkius.com/mcp/paperless-ngx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
