# Webiny CMS MCP Server

Manage content models, entries, and GraphQL workflows on Webiny — the enterprise open-source headless CMS.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/webiny-cms)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Webiny CMS** instance to any AI agent and manage your headless content infrastructure through natural conversation.

### What you can do

- **Content Lifecycle** — Create, update, publish, and delete content entries for any model directly from your agent
- **Model Discovery** — List all entries for specific content models and browse available data structures using introspection
- **Advanced GraphQL** — Execute raw GraphQL queries or mutations for custom logic and complex nested data operations
- **Revision Control** — Retrieve specific entry details by ID to inspect metadata and field-level property values
- **API Management** — Discover available types, fields, and models in your current environment through automated introspection
- **Global Config** — Verify high-level tenant settings and configurations to ensure your CMS environment is healthy
- **Multi-Locale Support** — Seamlessly manage content across different language locales (e.g., en-US, pt-BR)

### How it works

1. Subscribe to this server
2. Enter your Webiny API Domain and Access Token
3. Start managing your content models through Claude, Cursor, or any MCP-compatible client

No more manual JSON drafting in GraphQL playgrounds. Your AI agent becomes your content operations manager.

### Who is this for?

- **Content Managers** — update and publish entries across multiple models and locales without manual data entry
- **Headless Developers** — test GraphQL queries and verify content model introspection through chat
- **Marketing Teams** — quickly browse content items and verify publication status for different campaigns
- **CMS Administrators** — monitor tenant settings and audit content revisions through simple commands


## Available Tools
- **create_cms_entry**: Provide the singular model name and field data as a JSON object.

Creates a new draft entry for a content model
- **delete_cms_entry**: This action is irreversible.

Permanently deletes a content entry revision
- **execute_graphql_query**: Specify api_type (manage, read, preview) and locale.

Executes a raw GraphQL query or mutation against the Webiny CMS API
- **get_api_introspection**: Retrieves the GraphQL schema introspection for the Webiny instance
- **get_model_entry_details**: ID refers to the specific revision.

Retrieves details for a specific content model entry
- **get_tenant_config**: Retrieves global settings for the Webiny tenant
- **list_model_entries**: Provide the model plural name (e.g. "Articles"). Specify api_type (manage for drafts, read for live).

Lists all entries for a specific content model in Webiny
- **publish_cms_entry**: Provide the specific revision ID.

Publishes a draft entry, making it available via the "read" API
- **update_cms_entry**: Provide the entry ID and a JSON object containing the field updates.

Updates fields of an existing content entry revision


## Installation & Usage

To install and use the **Webiny CMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webiny-cms](https://vinkius.com/mcp/webiny-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
