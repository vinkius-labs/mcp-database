# Payload CMS MCP Server

Manage your Payload CMS instance — query collections, inspect documents, and manage content directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/payload-cms-extended)

## Overview
**Category:** developer-tools
**Tools Count:** 11

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


## Installation & Usage

To install and use the **Payload CMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payload-cms-extended](https://vinkius.com/mcp/payload-cms-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
