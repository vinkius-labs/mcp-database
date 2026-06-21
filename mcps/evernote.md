# Evernote MCP Server

Manage personal notes via Evernote — create and search notes, handle notebooks and tags, and monitor account quotas directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/evernote)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Evernote** account to any AI agent and take full control of your personal knowledge management and note-taking workflows through natural conversation.

### What you can do

- **Note & Content Orchestration** — Retrieve the full body and metadata of any note by GUID, including ENML body content and nested attachment attributes natively
- **Semantic & Syntax Search** — Execute powerful queries across all notebooks using Evernote's advanced syntax (keywords, tag filters, creation dates) to find information instantly
- **Notebook Management** — List all notebooks and retrieve detailed metadata including note counts and stack assignments to browse your workspace hierarchy
- **Live Note Creation** — Provision new notes inside specific notebooks by providing titles and plain-text or ENML content for immediate cross-device synchronization
- **Categorical Tagging** — Enumerate explicitly defined tags and manage nested tag hierarchies to filter and organize your personal database strictly
- **Account & Quota Oversight** — Fetch authenticated profile information including account tier, service level, and real-time quota usage to monitor system limits
- **Metadata Auditing** — Retrieve structural notebook representations and identify default status boundaries to manage your organizational topology flawlessly

### How it works

1. Subscribe to this server
2. Enter your Evernote Developer Token (found in your Evernote Account Settings > Developer Token)
3. Start managing your notes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — search for research notes and organize meeting minutes using natural language
- **Writers & Researchers** — create and update drafts and manage tag hierarchies without opening the Evernote app
- **Project Managers** — audit notebook stacks and monitor team contribution counts through natural conversation
- **Developers** — test and debug Evernote ENML rendering and note synchronization logic in real-time


## Available Tools
- **list_notebooks**: Use this to discover available notebooks before listing notes within them.

Retrieve all Evernote notebooks for the authenticated account
- **get_notebook**: Fetch detailed metadata for a specific Evernote notebook by its GUID
- **create_notebook**: Returns the newly created notebook GUID and metadata.

Create a new Evernote notebook
- **list_notes**: Use en.get_note to fetch full content.

List up to 50 notes inside a specific Evernote notebook
- **get_note**: The content is returned in Evernote Markup Language (ENML).

Retrieve the full content and metadata of a single Evernote note by GUID
- **create_note**: The note is immediately synced and available across all Evernote clients.

Create a new note inside a specified Evernote notebook
- **update_note**: This triggers a sync and increments the updateSequenceNum.

Update the title and/or content of an existing Evernote note
- **search_notes**: Returns matching note metadata.

Search across all Evernote notes using Evernote's powerful query syntax
- **list_tags**: Useful for filtering and organizing notes.

Retrieve all tags defined in the Evernote account
- **get_user**: Get profile information for the currently authenticated Evernote user


## Installation & Usage

To install and use the **Evernote** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/evernote](https://vinkius.com/mcp/evernote)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
