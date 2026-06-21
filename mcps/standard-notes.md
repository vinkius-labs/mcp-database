# Standard Notes MCP Server

Connect your AI to the Standard Notes encrypted ecosystem. Sync items natively, modify protected notes, and manage tags seamlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/standard-notes)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Seamlessly integrate your highly secure **Standard Notes** environments directly into your local AI workflows. Eliminate the friction of manually transferring encrypted data or research logs into your conversational interface. Empower your assistant to execute encrypted synchronizations, draft new secure notes, and systematically organize your knowledge base with precise tag management across your entire architecture.

### What you can do

- **Knowledge Retrieval** — Securely list your encrypted notes via `list_notes` or retrieve specific detailed payloads using the `get_item_details` routine.
- **Automated Drafting** — Command the agent to generate new structural content and save it securely via `create_note`, or surgically update existing drafts through `update_note`.
- **Vault Maintenance** — Maintain a clean workspace by permanently removing deprecated assets via `delete_item`, and keep local context synchronized with the official server using `sync_items`.
- **Taxonomy & Organization** — Streamline categorization by generating new organizational folders with `create_tag`, retrieving current structures with `list_tags`, and associating tags to specific items utilizing `tag_note`.

### How it works

1. Attach the Standard Notes MCP integration securely to your AI terminal.
2. Configure your endpoint URL (Official Cloud or Self-Hosted) along with your valid JWT Access Token.
3. Instruct your AI: "Retrieve the 'Project Alpha' note, update its contents with today's action items, and assign it the 'Priority' tag."

### Who is this for?

- **Privacy-focused Researchers** — Aggregate massive data logs using AI to pull notes, summarize them locally, and append new research securely without compromising client-side architecture.
- **Knowledge Architects & PKM Users** — Orchestrate seamless taxonomy alignments by instructing the AI to methodically analyze and map untagged notes.
- **System Administrators** — Automate the documentation of server incidents or deployment logs directly into a self-hosted encrypted database.


## Available Tools
- **create_note**: Provide plaintext title and text; encryption is handled by the sync layer.

Creates a new encrypted note
- **create_tag**: Creates a new tag
- **delete_item**: This action is irreversible.

Permanently deletes an item (note, tag, or extension) by UUID
- **get_auth_parameters**: Retrieves authentication parameters for an account email
- **get_item_details**: Retrieves a specific item (note, tag, or extension) by UUID
- **list_notes**: Note content remains encrypted until decrypted with user keys.

Lists all encrypted notes
- **list_tags**: Lists all tags defined in the account
- **sync_items**: Use the sync_token from the previous response.

Performs a Standard Notes sync operation
- **tag_note**: Requires both the tag UUID and the note UUID.

Associates a tag with a note
- **update_note**: Updates an existing note by UUID


## Installation & Usage

To install and use the **Standard Notes** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/standard-notes](https://vinkius.com/mcp/standard-notes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
