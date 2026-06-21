# Meilisearch MCP Server

Manage your Meilisearch instance — handle indexes, documents, and search configurations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/meilisearch)

## Overview
**Category:** loved-by-devs
**Tools Count:** 44

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


## Installation & Usage

To install and use the **Meilisearch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meilisearch](https://vinkius.com/mcp/meilisearch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
