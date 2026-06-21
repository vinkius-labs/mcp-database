# Zotero MCP Server

Manage your research library via Zotero — list collections, search items, and organize references directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zotero)

## Overview
**Category:** productivity
**Tools Count:** 23

## Description
Connect your **Zotero** library to any AI agent and take full control of your research workflow through natural conversation.

### What you can do

- **Collections & Organization** — List top-level collections, subcollections, and specific collection details to navigate your library structure.
- **Item Management** — Query all items, including notes and attachments, with support for advanced filtering by type, tag, or keyword.
- **Metadata Inspection** — Fetch complete bibliographic data, creator information, and publication details for any specific item.
- **Tags & Publications** — Access your personal publications and manage tags to categorize your research effectively.
- **Group Libraries** — Seamlessly switch between your personal library and shared group libraries using specific IDs.

### How it works

1. Subscribe to this server
2. Enter your Zotero API Key and User ID
3. Start managing your references from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find citations and organize papers without leaving your writing environment.
- **Students** — manage reading lists and extract metadata for bibliographies through simple chat.
- **Knowledge Workers** — centralize your document management and reference tracking within your AI-powered workspace.


## Available Tools
- **create_items**: Use get_new_item_template first to get the correct schema.

Create new items in the Zotero library
- **delete_item**: Delete a single item
- **delete_items**: Delete multiple items (up to 50)
- **get_collection**: Get a specific collection by key
- **get_deleted**: Get deleted objects since a specific library version
- **get_item**: Get a specific item by key
- **get_item_type_fields**: List valid fields for a specific item type
- **get_new_item_template**: Get a JSON template for creating a new item of a specific type
- **get_tag**: Get tags matching a specific name
- **list_collection_items**: List items in a specific collection
- **list_collections**: List all collections in the Zotero library
- **list_item_children**: List child items (notes, attachments) for a specific item
- **list_item_fields**: List all available Zotero item fields
- **list_item_tags**: List tags for a specific item
- **list_item_types**: List all available Zotero item types
- **list_items**: List items in the Zotero library
- **list_publications**: List items in My Publications
- **list_subcollections**: List subcollections of a specific collection
- **list_tags**: List all tags in the library
- **list_top_collections**: List top-level collections in the Zotero library
- **list_top_items**: List top-level items in the Zotero library
- **list_trash_items**: List items in the trash
- **update_item**: Update an existing item (Partial Update / PATCH)


## Installation & Usage

To install and use the **Zotero** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zotero](https://vinkius.com/mcp/zotero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
