# Zotero MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zotero)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your research library via Zotero — list collections, search items, and organize references directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zotero** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my top-level collections in Zotero."

**🤖 AI Agent:**
> I've retrieved your top-level collections. You have 'Thesis Research' (Key: A1B2C3D4), 'Machine Learning Papers' (Key: E5F6G7H8), and 'General Reading' (Key: I9J0K1L2). Which one would you like to explore?

---

**👤 You:**
> "Search for items in my library with the tag 'artificial-intelligence'."

**🤖 AI Agent:**
> Searching for items tagged 'artificial-intelligence'... I found 3 items, including 'Attention Is All You Need' and 'Deep Learning Review'. Would you like the full details for any of these?

---

**👤 You:**
> "Get the complete bibliographic details for item key ABCD1234."

**🤖 AI Agent:**
> Fetching details for item ABCD1234... This is a journal article titled 'Neural Networks for Beginners' by Smith et al. (2023), published in the Journal of AI Research. It currently has 5 tags and 2 attached notes.


## ❓ FAQ

**Q: Can I search for specific items in my library using keywords?**
Yes! Use the `list_items` tool with the `q` parameter. It performs a quick search across titles and creators to find exactly what you need.

**Q: How do I view the subcollections nested inside a main collection?**
Simply use the `list_subcollections` tool and provide the `collection_key` of the parent collection. The agent will return all nested folders.

**Q: Does this support shared group libraries or only my personal library?**
It supports both! Most tools, like `list_collections` or `list_items`, accept an optional `group_id`. If provided, the agent will query that specific group library instead of your personal one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zotero](https://vinkius.com/mcp/zotero)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zotero** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zotero` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zotero** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zotero": {
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
