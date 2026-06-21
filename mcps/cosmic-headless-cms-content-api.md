# Cosmic (Headless CMS & Content API) MCP Server

Manage your content, media, and object types via Cosmic — list objects, create content, and handle media assets directly through any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cosmic-headless-cms-content-api)

## Overview
**Category:** developer-tools
**Tools Count:** 21

## Description
Connect your **Cosmic** headless CMS to any AI agent to manage your content infrastructure through natural language. Cosmic provides a powerful API-first approach to content management, and this MCP server brings those capabilities directly to your AI workflows.

### What you can do

- **Content Management** — Create, read, update, and delete objects across your buckets with full metadata support.
- **Media Library** — List, upload, and manage your media assets including images, videos, and documents.
- **Schema Control** — Manage object types and structures programmatically to maintain your content model.
- **Version Control** — Access and manage revisions to track changes and restore previous versions of your content.
- **Batch Operations** — Execute multiple object operations in a single request for high-efficiency updates.

### How it works

1. Subscribe to this server
2. Provide your Cosmic Bucket Slug, Read Key, and Write Key
3. Start managing your headless CMS from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Quickly query content structures or update metadata without leaving the code editor.
- **Content Managers** — Use AI to draft new objects, organize media, or audit existing content entries.
- **Product Teams** — Automate content updates and maintain consistency across multiple buckets.


## Available Tools
- **batch_objects**: Perform batch operations on Objects (Max 25)
- **create_media**: Create/Upload Media
- **create_object**: Create a new Object
- **create_object_type**: Create a new Object Type
- **create_revision**: Add a Revision for an Object
- **delete_media**: Delete Media
- **delete_object**: Delete an Object
- **delete_object_type**: Delete an Object Type
- **get_agent_conversation_history**: Get history for a specific Agent conversation
- **get_object**: Get a single Object by ID
- **get_object_type**: Get a single Object Type by slug
- **get_revision**: Get a single Revision for an Object
- **list_agent_conversations**: List conversations for an AI Agent
- **list_media**: List Media in a Cosmic Bucket
- **list_object_types**: List Object Types in a Cosmic Bucket
- **list_objects**: Use the query parameter (URL encoded JSON) to filter results.

List Objects in a Cosmic Bucket
- **list_revisions**: Get Revisions for an Object
- **send_agent_message**: Send a message to an AI Agent
- **update_media**: Update Media metadata
- **update_object**: Update an existing Object
- **update_object_type**: Update an Object Type


## Installation & Usage

To install and use the **Cosmic (Headless CMS & Content API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cosmic-headless-cms-content-api](https://vinkius.com/mcp/cosmic-headless-cms-content-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
