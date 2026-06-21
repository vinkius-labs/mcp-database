# Payload CMS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payload-cms-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/payload-cms-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/payload-cms-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your Payload CMS instance — query collections, inspect documents, and manage content directly from your AI agent.

## Description
Connect your **Payload CMS** instance to any AI agent and take full control of your headless content management and application framework through natural conversation.

### What you can do

- **Collection Discovery** — List all available collections and globals defined in your TypeScript schema
- **Advanced Querying** — Find specific documents using complex filters, pagination, and sorting directly from the chat
- **Document Inspection** — Fetch full JSON payloads for specific documents to understand relationships and data structures
- **Content Management** — Create or update entries in your database without leaving your AI interface
- **Schema Awareness** — Understand your data model and field types to ensure accurate content operations

### How it works

1. Subscribe to this server
2. Enter your Payload CMS Instance URL and API Key
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

No more switching between your code editor and the Payload Admin panel to verify field names or check entry IDs. Your AI acts as a specialized content engineer.

### Who is this for?

- **Developers** — query your local or production database to verify data structures while coding
- **Content Managers** — quickly find and update specific entries across multiple collections using natural language
- **DevOps Engineers** — inspect system globals and configuration settings across different environments


## Available Tools
- **create_document**: Create a new document in a collection
- **delete_document**: Delete a document
- **get_document**: Get a single document by ID
- **get_global**: Get global data
- **get_me**: Get current authenticated user details
- **list_documents**: Supports optional query string for filtering, sorting, and pagination.

List documents from a Payload CMS collection
- **login_user**: Login a user to get an authentication token
- **logout_user**: Logout the current user
- **refresh_token**: Refresh authentication token
- **update_document**: Update an existing document
- **update_global**: Update global data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Payload CMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the collections available in my Payload CMS."

**🤖 AI Agent:**
> I've accessed your Payload instance. You have 4 active collections: 'Users', 'Posts', 'Categories', and 'Media'. You also have a global called 'Site-Settings'. Which one would you like to explore?

---

**👤 You:**
> "Find the post with the slug 'announcing-mcp-support' in the 'posts' collection."

**🤖 AI Agent:**
> Searching... I found one document in 'posts' matching that slug. The ID is `65a2b...`, the status is 'published', and it was last updated on Oct 24th. Would you like the full content of this post?

---

**👤 You:**
> "Get the full details for document ID 64f123456789 in the 'products' collection."

**🤖 AI Agent:**
> Retrieving document... Here are the details for 'Wireless Headphones' (ID: 64f123456789). It has a price of $199, stock level of 45, and is linked to the 'Electronics' category. I've also retrieved the associated image metadata.


## Installation & Usage

To install and use the **Payload CMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payload-cms-extended](https://vinkius.com/mcp/payload-cms-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
