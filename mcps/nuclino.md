# Nuclino MCP Server

Equip your AI agent with full read/write access to your Nuclino workspaces, teams, and items — the unified tool for knowledge, docs, and projects.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nuclino)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Connect your **Nuclino** account to your AI agent and seamlessly interact with your company's unified workspace for knowledge, docs, and projects.

### What you can do

- **Teams & Workspaces** — Rapidly list all teams you are part of, and enumerate the nested workspaces and collections to understand your organization's hierarchy.
- **Search & Query** — Perform global fuzzy searches using `search_items` to track down specific documents, notes, or project pages across the entire knowledge base.
- **Read Items & Files** — Read the exact content configuration of any item (document) via `get_item`, and list attachments or files uploaded to the platform.
- **Record Creation** — Instantly create new items natively inside your workspace using natural language.
- **Telemetrics** — Enumerate members and structural fields within your Nuclino domain to keep the agent aware of context and owners.

### How it works

1. Subscribe to this server
2. Enter your Nuclino Personal API Key
3. Start querying your company wiki and project trackers from Claude, Cursor, or your preferred AI client

### Who is this for?

- **Knowledge Managers** — quickly search the internal wiki, read past guidelines, and append meeting notes to workspaces automatically.
- **Engineering Teams** — access technical documentation and specs without leaving your IDE.
- **Project Managers** — track deliverables, create new planning documents, and monitor active users.


## Available Tools
- **list_teams**: Use this as the entry point to discover available root organizational unit IDs traversing down into workspaces.

List all organizational Teams the authenticated user belongs to
- **list_workspaces**: Returns internal workspace UUIDs essential for scoping later item queries.

List all isolated Workspaces mapped within a specific Team
- **list_items**: Used to enumerate top-level document UUIDs, titles, and creation metadata natively spanning a specific Workspace layer.

List all standard knowledge items (pages) in a Workspace
- **get_item**: Retrieve the exact Markdown payload and configuration of an Item
- **create_item**: Triggers real-time replication creating permanent Wiki documentation.

Write a brand new knowledge Item / Page into a Workspace
- **update_item**: Alters the sync tree immediately appending new wiki edits.

Overwrite active partial Markdown states inside a listed Item
- **delete_item**: Always confirm with the user heavily before destroying knowledge.

Irreversibly delete a structural Nuclino Item
- **search_items**: Use to uncover unknown UUIDs.

Execute an indexed semantic search globally across a Team
- **list_collections**: Used to trace the document relationship graph paths visually within a target Workspace.

List Collections (grouping directories) segmenting a Workspace
- **list_fields**: Used to understand standard taxonomy dimensions applicable against Items.

Map customizable structured property fields globally binding a Team
- **list_users**: Enumerate human identities attached globally onto a Team
- **list_files**: Exposes pure URL bindings mapping binary data records back to object storage.

List physical attachments explicitly bolted onto an Item


## Installation & Usage

To install and use the **Nuclino** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nuclino](https://vinkius.com/mcp/nuclino)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
