# Sanity MCP Server

Manage your Sanity Content Lake via AI — execute GROQ queries, manage documents, and handle media assets directly from your agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sanity)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Sanity** project to any AI agent and take full control of your Content Lake through natural conversation.

### What you can do

- **GROQ Queries** — Execute powerful Graph-Relational Object Queries to fetch exactly the content you need
- **Document Management** — Create, read, update, patch, and delete documents of any schema type
- **Schema Insights** — List unique schema types and count entity nodes dynamically
- **Media Assets** — Browse and manage images and file assets uploaded to your project
- **Bulk Operations** — Run raw Sanity mutations for complex, multi-document transactions

### How it works

1. Subscribe to this server
2. Enter your Sanity Project ID, Dataset, API Version, and API Token
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a headless CMS power-user, perfectly capable of navigating references and transforming content on the fly.

### Who is this for?

- **Developers** — prototype GROQ queries, audit schema types, and run quick data migrations
- **Content Editors** — bulk edit fields, update taxonomy, and manage assets without leaving your chat
- **Product Managers** — query content stats and generate instant reports on published vs. draft documents


## Available Tools
- **list_typed_documents**: g., "post", "author").

Lists all documents of a specific type
- **count_entity_nodes**: Counts the number of documents of a specific type
- **list_unique_schema_types**: Retrieves a list of all unique document types present in the dataset
- **create_cms_document**: Specify the type and provide attributes as a JSON object.

Creates a new document in the CMS
- **get_document_details**: Retrieves full details for a specific document by ID
- **list_media_assets**: Lists all image and file assets uploaded to Sanity
- **patch_cms_document**: Provide a JSON object of fields to set.

Updates specific fields of an existing document
- **run_groq_query**: Executes a GROQ (Graph-Relational Object Queries) query
- **run_raw_mutation**: Provide a JSON array of mutation objects.

Executes a raw Sanity mutation
- **wipe_cms_document**: This action is irreversible.

Permanently deletes a document from the CMS


## Installation & Usage

To install and use the **Sanity** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sanity](https://vinkius.com/mcp/sanity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
