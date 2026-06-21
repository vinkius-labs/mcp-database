# Simplenote MCP Server

Manage your Simplenote notes directly from your AI assistant. Create, search, edit, and organize plain-text notes without leaving the conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/simplenote)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect your AI assistant to your Simplenote account for seamless note management. The **Simplenote MCP** enables your LLM to act as a personal note-taking assistant with full read and write access to your notes.

### What you can do

- **Browse & Search** — List all your notes with `list_notes` or find specific content using `search_notes`. Explore note history with `get_note_version` to review previous edits
- **Create & Edit** — Capture ideas instantly with `create_note` or update existing notes using `update_note`, all through natural conversation
- **Organize & Clean Up** — View your tag taxonomy with `list_tags` or permanently remove notes with `delete_note`

### How it works

1. Add this server to your MCP-compatible AI client
2. Configure your `SIMPLENOTE_APP_ID` and `SIMPLENOTE_TOKEN` in the credential settings
3. Start managing notes conversationally: "List my recent notes and search for anything mentioning 'project roadmap'"


## Available Tools
- **create_note**: Provide the full text content.

Creates a new note
- **delete_note**: This action is irreversible.

Permanently deletes a note
- **get_note_details**: Retrieves details for a specific note
- **get_note_version**: Requires note key and version number.

Retrieves a specific historical version of a note
- **list_notes**: Returns note keys and a preview of the content.

Lists all notes in Simplenote
- **list_tags**: Lists all tags used in your notes
- **search_notes**: Searches for notes containing specific text
- **update_note**: Requires the note key.

Updates an existing note


## Installation & Usage

To install and use the **Simplenote** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplenote](https://vinkius.com/mcp/simplenote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
