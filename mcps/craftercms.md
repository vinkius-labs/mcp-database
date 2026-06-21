# CrafterCMS MCP Server

Manage and query content from CrafterCMS — fetch pages, components, and trees, execute GraphQL/OpenSearch queries, and manage engine cache directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/craftercms)

## Overview
**Category:** developer-tools
**Tools Count:** 12

## Description
Connect your **CrafterCMS** instance to any AI agent to streamline your content management and delivery workflows. This server provides deep integration with Crafter Engine, allowing you to inspect content structures, perform advanced searches, and manage site contexts through natural language.

### What you can do

- **Content Retrieval** — Fetch specific items, components, or entire folder hierarchies using `get_item`, `get_component`, and `get_tree`.
- **Navigation & Structure** — Explore site architecture with `get_navigation_tree`, `get_breadcrumb`, and `get_children` to understand content relationships.
- **Advanced Querying** — Execute complex `graphql` queries against your content schema or perform raw `search` operations using OpenSearch JSON syntax.
- **URL Transformation** — Use `transform_url` to apply specific logic to content paths for different delivery environments.
- **Engine Management** — Monitor system health with `get_status` and perform administrative actions like `clear_cache` or `rebuild_context`.

### How it works

1. Subscribe to this server
2. Provide your CrafterCMS Base URL and Site ID
3. Enter your Access and Management tokens
4. Start querying your headless content directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Query content schemas and test GraphQL queries directly from the IDE without switching to the Crafter Studio.
- **Content Managers** — Quickly verify content status, hierarchy, and metadata across different site environments.
- **DevOps & Admins** — Monitor engine status and trigger cache invalidations or context rebuilds via simple commands.


## Available Tools
- **clear_cache**: Requires management token.

Clear the Crafter Engine cache
- **get_breadcrumb**: Get breadcrumb navigation for a URL
- **get_children**: List children of a folder in CrafterCMS
- **get_component**: Render and retrieve a specific component
- **get_item**: Get a single item from CrafterCMS content store
- **get_navigation_tree**: Get navigation tree
- **get_status**: Get Crafter Engine monitoring status
- **get_tree**: Get complete hierarchy under a folder
- **graphql**: Execute a GraphQL query
- **rebuild_context**: Requires management token.

Rebuild the Crafter Engine context
- **search**: Execute an OpenSearch JSON query
- **transform_url**: Transform a URL using a specific transformer


## Installation & Usage

To install and use the **CrafterCMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/craftercms](https://vinkius.com/mcp/craftercms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
