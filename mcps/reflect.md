# Reflect MCP Server

Equip your AI to read, write, and explore your networked thought graph in Reflect Notes securely via their API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/reflect)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Reflect** account securely to your AI agent via their developer API. This integration grants your AI the ability to directly explore your networked thought graph, lookup personal notes, manage book highlights, and append daily thoughts asynchronously from your conversation interface.

### What you can do

- **Explore Your Graph** — Direct your AI to investigate connected insights within your Reflect graphs (`list_graphs`). Request lists of your notes (`list_notes`) or retrieve the specific Markdown content of a single note (`get_note`).
- **Capture Ideas Instantly** — Ask the agent to establish new permanent notes (`create_note`) or quickly dump conversational insights, summaries, and tasks straight into your daily note (`append_daily_note`).
- **Analyze Connections** — Instruct the AI to map out your thoughts by retrieving all backlinks pointing to a specific subject (`get_backlinks`).
- **Save Links & Books** — Let your AI automatically bookmark URLs (`create_link`), browse your saved bookmarks (`list_links`), or explore your imported library of book highlights (`list_books`).

### How it works

1. Authorize the Reflect MCP plugin in your active extensions.
2. Obtain your personal OAuth Access Token from your Reflect application settings (reflect.app/developer/oauth) and embed it securely into the integration.
3. Chat naturally with your AI, prompting tasks like "Append a summary of this conversation to my daily note" or "List all notes connected to 'AI Strategy'."

### Who is this for?

- **Researchers & Writers** — Interactively synthesize information. Have your AI recall connected ideas from your graph while you brainstorm, without switching apps.
- **Founders & Execs** — Seamlessly capture action items. Simply ask your assistant to log decisions and links directly into today's daily note.
- **Knowledge Workers** — Transform your AI into a personalized knowledge broker that understands your private context and highlights instantly.


## Available Tools
- **append_daily_note**: Optionally specify a list/heading name.

Appends Markdown text to today's daily note
- **create_link**: Reflect will automatically attempt to extract metadata.

Saves a new web link/bookmark to a Reflect graph
- **create_note**: Specify subject and Markdown content.

Creates a new note in a Reflect graph
- **get_backlinks**: Retrieves all notes that link to a specific note
- **get_current_user**: Retrieves profile details for the authenticated Reflect user
- **get_note**: Retrieves the full content and metadata of a Reflect note
- **list_books**: Lists all books saved or imported into Reflect
- **list_graphs**: Lists all Reflect graphs (workspaces) accessible by the user
- **list_links**: Lists all saved links (bookmarks) in a graph
- **list_notes**: Lists all notes within a specific Reflect graph


## Installation & Usage

To install and use the **Reflect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reflect](https://vinkius.com/mcp/reflect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
