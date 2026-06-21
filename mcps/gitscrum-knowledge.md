# GitScrum Knowledge MCP Server

Build and query knowledge bases via GitScrum — manage notes as agent memory, maintain wiki pages, communicate through discussions, and search across all resources from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-knowledge)

## Overview
**Category:** collaboration
**Tools Count:** 28

## Description
### What you can do

- **Agent memory via notes** — create, update, share, and organize notes as persistent AI memory with full revision history and folder management
- **Wiki knowledge base** — build and maintain project documentation with nested pages, markdown content, revision tracking, and restore capabilities
- **Team discussions** — create channels, send messages, search conversations, and reply in threads for structured team communication
- **Global search** — search across tasks, wiki pages, discussions, user stories, sprints, and notes in a single query
- **Knowledge versioning** — track how information evolves over time with note and wiki revision histories

### How it works

1. Subscribe to the GitScrum Knowledge integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Use your agent as a knowledge hub — store decisions in notes, document processes in wiki, discuss with the team, and search everything in natural language

Your agent becomes the central knowledge repository, bridging personal memory with team knowledge.

### Who is this for?

- **AI practitioners** — maintain persistent agent memory across sessions using notes as structured context
- **Technical writers** — manage wiki documentation with version control and search directly through conversation
- **Team leads** — foster asynchronous team communication and decision-tracking without platform switching


## Available Tools
- **create_channel**: Create a discussion channel
- **get_channel**: Get channel details
- **list_channels**: List discussion channels
- **list_discussions**: List all discussions in a project
- **create_note_folder**: E.g., "Agent Memory", "Architecture Decisions", "Meeting Notes".

Create a note folder
- **list_note_folders**: Use folders to categorize agent memory by topic or project.

List note folders
- **rename_note_folder**: Rename a note folder
- **channel_messages**: Get messages in a channel
- **search_channel_messages**: Search messages in a channel
- **send_message**: Useful for agents to communicate findings or status updates.

Send a message to a channel
- **create_note**: Use this as persistent agent memory: store decisions, context, meeting notes, or ADRs. Content supports full markdown.

Create a new note
- **delete_note**: Delete a note permanently
- **list_notes**: Perfect for agent memory — store context, decisions, and key information across sessions.

List all notes in the workspace
- **move_note_to_folder**: Move a note into a folder
- **note_revisions**: Useful for tracking how knowledge evolved over time.

Get note revision history
- **toggle_note_share**: Useful for publishing agent findings to the team.

Toggle note sharing visibility
- **update_note**: Use to append context or refine agent memory over time.

Update an existing note
- **reply_to_message**: Reply to a message in a thread
- **global_search**: Returns grouped results by resource type.

Search across all workspace resources
- **thread_replies**: Get thread replies for a message
- **create_wiki_page**: Supports nested pages via parent_uuid.

Create a wiki page
- **delete_wiki_page**: Delete a wiki page
- **get_wiki_page**: Get a wiki page with full content
- **list_wiki_pages**: Wiki pages support markdown and nested hierarchies.

List wiki pages in a project
- **restore_wiki_revision**: Restore a wiki page to a previous revision
- **wiki_revisions**: Get wiki page revision history
- **search_wiki**: Search wiki pages
- **update_wiki_page**: Update a wiki page


## Installation & Usage

To install and use the **GitScrum Knowledge** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-knowledge](https://vinkius.com/mcp/gitscrum-knowledge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
