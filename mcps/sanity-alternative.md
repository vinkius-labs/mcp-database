# Sanity MCP Server

Manage headless CMS content via Sanity — query documents with GROQ, create/update/delete content and manage datasets from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sanity-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 11

## Description
Connect your **Sanity** project to any AI agent and take full control of your content through natural conversation.

### What you can do

- **Content Queries** — List, search and retrieve documents by type or run custom GROQ queries
- **Content Management** — Create, update and delete documents with full schema support
- **Dataset Management** — List existing datasets and create new ones for staging/development
- **Asset Management** — Browse image assets and manage media library content
- **Team Management** — List project members and audit access permissions

### How it works

1. Subscribe to this server
2. Enter your Sanity Project ID, Dataset name and API Token
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

No more navigating the Sanity Studio to find documents or run GROQ queries. Your AI acts as a dedicated content operations assistant.

### Who is this for?

- **Content Teams** — quickly create and update content, search for specific documents and browse content collections
- **Developers** — run GROQ queries, manage schemas programmatically and audit project access
- **Editors** — search for content by keyword, review document details and manage media assets


## Available Tools
- **create_dataset**: Provide the dataset name (e.g. "staging", "development"). The dataset will be empty and ready for content. Dataset names must be lowercase alphanumeric.

Create a new Sanity dataset
- **create_document**: Requires a JSON object with _type and content fields. For example: {"_type": "post", "title": "Hello", "body": "World"}. Returns the created document with its generated ID.

Create a new Sanity document
- **delete_document**: Provide the document ID. WARNING: this action is irreversible.

Delete a Sanity document
- **get_document**: g. "drafts.abc123" or "abc123"). Returns the full document with all fields. Useful for inspecting individual content items.

Get a specific Sanity document by ID
- **list_datasets**: Datasets are isolated content collections within a project (e.g. "production", "staging", "development").

List all datasets in the Sanity project
- **list_documents**: g. "post", "product", "author") from the configured dataset. Each document returns its _id, content fields and metadata. Use this to browse content collections.

List documents of a specific type in Sanity
- **list_image_assets**: Each asset includes its _id, original filename, dimensions and metadata. Optionally set a limit. Useful for managing media library content.

List image assets in Sanity
- **list_users**: Useful for auditing project access and team management.

List project members in Sanity
- **query_documents**: Requires a GROQ query string. Optionally provide params as JSON for parameterized queries. Returns query results as an array. Example query: "*[_type == 'post' && publishedAt > $date]{title, slug}"

Run a GROQ query against Sanity
- **search_documents**: Optionally filter by document types and set a result limit. Returns matching documents with their full content.

Search documents in Sanity
- **update_document**: Requires the document ID and a JSON object with the fields to set. For example: {"title": "Updated Title", "status": "published"}. Only provided fields will be modified.

Update fields on a Sanity document


## Installation & Usage

To install and use the **Sanity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sanity-alternative](https://vinkius.com/mcp/sanity-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
