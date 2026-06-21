# Plone MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plone)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/plone-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/plone-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage Plone CMS content, users, and workflows directly from your AI agent—search, create, and update resources effortlessly.

## Description
Connect your **Plone** CMS instance to any AI agent to manage your enterprise content through natural conversation.

### What you can do

- **Content Management** — Search, retrieve, create, update, and delete content objects using paths and metadata.
- **User & Group Administration** — List and manage users and groups, including profile updates and creation.
- **Workflow Transitions** — Inspect current workflow states and trigger transitions to move content through its lifecycle.
- **Advanced Search** — Use full-text search, type filtering, and path-based queries to find exactly what you need.

### How it works

1. Subscribe to this server
2. Enter your Plone Instance URL and Personal Access Token
3. Start managing your CMS from Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex CMS hierarchies. Your AI acts as a content editor and site administrator.

### Who is this for?

- **Content Managers** — quickly update pages, create news items, and manage publication workflows without the web UI
- **Site Administrators** — manage users and groups or perform bulk content searches via natural language
- **Developers** — inspect content structures and metadata directly from the code editor


## Available Tools
- **create_content**: Create new content in Plone
- **create_group**: Create a new group
- **create_user**: Create a new user
- **delete_content**: Delete content from Plone
- **delete_group**: Delete a group
- **delete_user**: Delete a user
- **get_content**: Get a specific content object by path
- **get_group**: Get details for a specific group
- **get_user**: Get details for a specific user
- **get_workflow**: Get workflow status and history for content
- **list_groups**: List groups in Plone
- **list_users**: Requires Manager role.

List users in Plone
- **search_content**: Search for content in Plone
- **transition_workflow**: Trigger a workflow transition on content
- **update_content**: Supports partial updates.

Update existing content in Plone
- **update_group**: Update a group
- **update_user**: Update a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all Documents containing 'roadmap' in the /news folder."

**🤖 AI Agent:**
> I've searched the /news path. I found 2 documents: 'Product Roadmap 2024' and 'Q3 Engineering Roadmap'. Would you like to see the details of either one?

---

**👤 You:**
> "Create a new Folder titled 'Marketing 2025' at the root path."

**🤖 AI Agent:**
> Successfully created the folder 'Marketing 2025' at path /marketing-2025. You can now start adding content to it.

---

**👤 You:**
> "Get the content of the page at /about-us and show its current workflow state."

**🤖 AI Agent:**
> I've retrieved the page. The title is 'About Our Company' and its current workflow state is 'private'. Would you like to transition it to 'published'?


## Installation & Usage

To install and use the **Plone** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plone](https://vinkius.com/mcp/plone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
