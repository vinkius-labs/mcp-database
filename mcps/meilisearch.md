# Meilisearch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meilisearch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your Meilisearch instance — handle indexes, documents, and search configurations directly from your AI agent.

## Description
Connect your **Meilisearch** instance to any AI agent to automate your search engine management and data indexing workflows.

### What you can do

- **Index Management** — Create, list, update, and delete indexes. Perform atomic swaps between indexes for zero-downtime deployments.
- **Document Operations** — Add, update, or replace documents in bulk. Retrieve specific documents by ID or list them with advanced filtering and sorting.
- **Granular Deletion** — Remove documents individually, in batches, or by applying complex filter expressions to clean up your data.
- **Metadata Inspection** — Fetch detailed metadata for your indexes and documents to monitor your search engine's state.

### How it works

1. Subscribe to this server
2. Enter your Meilisearch Instance URL and API Key
3. Start managing your search data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Index new data or debug search results directly from the code editor.
- **Data Engineers** — Automate index maintenance and document synchronization tasks.
- **Content Managers** — Quickly verify if specific content is correctly indexed without using a dedicated dashboard.


## Available Tools
- **add_documents**: Add or replace documents in an index
- **cancel_tasks**: Cancel pending or processing tasks
- **chat_completion**: Request a chat completion from a workspace
- **configure_experimental_features**: Enable or disable experimental features
- **create_dump**: Trigger the creation of a Meilisearch dump
- **create_index**: Create a new index
- **create_key**: Create a new API key
- **create_snapshot**: Trigger the creation of a Meilisearch snapshot
- **delete_all_documents**: Delete all documents in an index
- **delete_document**: Delete a single document
- **delete_documents_batch**: Delete multiple documents by ID
- **delete_documents_by_filter**: Delete documents matching a filter
- **delete_dynamic_search_rule**: Delete a dynamic search rule
- **delete_index**: Delete an index
- **delete_key**: Delete an API key
- **delete_tasks**: Delete finished tasks
- **get_batch**: Get details of a specific batch
- **get_document**: Get a specific document by ID
- **get_health**: Check the health of the Meilisearch instance
- **get_index_stats**: Get stats of a specific index
- **get_index**: Get metadata for a specific index
- **get_key**: Get details of a specific API key
- **get_settings**: Get all settings of an index
- **get_stats**: Get stats of all indexes and database size
- **get_task**: Get details of a specific task
- **get_version**: Get the version of the Meilisearch instance
- **list_batches**: List task batches
- **list_chats**: List chat workspaces
- **list_documents**: List documents in an index
- **list_dynamic_search_rules**: List dynamic search rules for an index
- **list_experimental_features**: List the status of experimental features
- **list_indexes**: List all Meilisearch indexes
- **list_keys**: List API keys
- **list_tasks**: List asynchronous tasks
- **multi_search**: Perform multiple search queries in a single call
- **reset_settings**: Reset all settings of an index to defaults
- **search_documents**: Search for documents in an index
- **set_dynamic_search_rule**: Create or update a dynamic search rule
- **similar_documents**: Find documents similar to a given document ID
- **swap_indexes**: Swap multiple indexes atomically
- **update_documents**: Add or update documents (partial update)
- **update_index**: Update an index primary key
- **update_key**: Update an API key name or description
- **update_settings**: Update settings of an index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meilisearch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Meilisearch indexes and their primary keys."

**🤖 AI Agent:**
> I've retrieved your indexes. You have 3 active indexes: 'movies' (primary key: 'id'), 'books' (primary key: 'isbn'), and 'products' (primary key: 'sku').

---

**👤 You:**
> "Add these three product documents to the 'products' index: [JSON data]."

**🤖 AI Agent:**
> I've initiated the document addition for the 'products' index. The task has been enqueued with UID 452. You can check the status to confirm when the indexing is complete.

---

**👤 You:**
> "Get the document with ID 'prod_99' from the 'products' index, but only show the 'name' and 'price' fields."

**🤖 AI Agent:**
> Here is the requested document from 'products': { "name": "Wireless Headphones", "price": 99.99 }.


## ❓ FAQ

**Q: Can I delete documents based on a specific condition or category?**
Yes! You can use the `delete_documents_by_filter` tool. Just provide the index UID and a filter expression (e.g., 'category = electronics') to remove all matching documents at once.

**Q: How do I perform a zero-downtime index update?**
You can use the `swap_indexes` tool. This allows you to swap the names of two or more indexes atomically, ensuring your search remains active while you switch to a newly populated index.

**Q: Is it possible to retrieve only specific fields from a document?**
Absolutely. When using `get_document` or `list_documents`, you can provide a comma-separated list of `fields` to return, reducing the payload size and focusing on the data you need.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meilisearch](https://vinkius.com/mcp/meilisearch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meilisearch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `meilisearch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meilisearch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meilisearch": {
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
