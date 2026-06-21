# Notion MCP Server

Unified AI interface for your Notion workspace — search pages, query databases, and manage blocks via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/notion)

## Overview
**Category:** loved-by-devs
**Tools Count:** 14

## Description
Unlock the full potential of your connected workspace by linking **Notion** to your AI agent. This integration transforms Notion from a static documentation hub into a dynamic, queryable engine for your AI workflows. Your agent can now perform global fuzzy searches to locate misplaced documents, query structured databases to extract tabular data, and even read deep into nested block hierarchies to summarize project specs or meeting notes. Whether you're automating task creation or retrieving team knowledge, your agent acts as an intelligent librarian for your entire Notion domain.

### What you can do

- **Global Search** — Rapidly find pages and databases across your workspace by title or content using fuzzy text matching.
- **Database Orchestration** — Query databases to read structured data rows or fetch the exact schema defining your trackers.
- **Deep Content Reading** — Access metadata and dive into nested paragraphs, lists, and images using advanced block retrieval.
- **Record Creation** — Programmatically create new pages or insert data rows directly inside specific Notion containers.
- **Identity Mapping** — Enumerate all workspace users and bots to accurately map assignee tags to team members.

### How it works

1. Subscribe to this server
2. Enter your Notion Internal Integration Secret
3. Start querying your company wiki and project trackers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Productivity Experts** — quickly search the internal wiki, read deep project specs, and append notes to central databases.
- **Software Teams** — query central sprint trackers and create new tasks without ever leaving your development environment.
- **Ops Managers** — build automated AI reporting flows by safely reading the real-time state of active rows and users.
- **Knowledge Workers** — retrieve specific documentation fragments instantly through natural language conversation.


## Available Tools
- **create_database**: Properties define columns. Minimum: provide a title property with type "title".

Create a new Notion database inside a page
- **append_block_children**: ) to the end of a page or nested block. Provide blocks as a JSON array of Notion block objects. Example for a paragraph: [{"type":"paragraph","paragraph":{"rich_text":[{"type":"text","text":{"content":"Hello world"}}]}}]

Append content blocks to a Notion page or block
- **archive_page**: Archive/Delete a Notion Page
- **get_blocks**: Read hierarchical textual content under a Page
- **create_page**: Insert a new row/page inside a Database
- **delete_block**: ) from a page. This action is irreversible — the block and all nested children are permanently deleted.

Permanently delete a Notion block
- **get_database**: ) defining rows within a Database.

Retrieve the schema definition of a Database
- **get_page**: Does NOT fetch body text.

Retrieve metadata properties for a single Notion Page
- **list_users**: Enumerate workspace members and bots
- **query_database**: Read structured data rows from a Notion Database
- **search_databases**: Essential for tracking down Database UUIDs.

Fuzzy text search globally across Notion workspace Databases
- **search_pages**: Necessary to locate Page UUIDs rapidly.

Fuzzy text search globally across Notion workspace pages
- **update_page_properties**: ) using the Notion properties schema. Provide the properties as a JSON object matching the Notion API property format.

Update arbitrary properties on a Notion page
- **update_page_title**: Update the title of a Notion Page


## Installation & Usage

To install and use the **Notion** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notion](https://vinkius.com/mcp/notion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
