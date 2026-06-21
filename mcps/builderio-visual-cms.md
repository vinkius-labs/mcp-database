# Builder.io (Visual CMS) MCP Server

Manage Builder.io content, assets, and models via AI — fetch entries, update data, and query GraphQL APIs directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/builderio-visual-cms)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Builder.io** space to any AI agent and take full control of your visual CMS and headless content through natural conversation.

### What you can do

- **Content Management** — Fetch entries from any model using `get_content` or retrieve pre-rendered HTML for components with `get_html`.
- **Write Operations** — Create, update, or delete content entries programmatically using the Write API tools like `create_content` and `update_content`.
- **Advanced Querying** — Execute complex GraphQL queries against the Content API or perform administrative tasks using `admin_graphql`.
- **Asset Handling** — Upload new media assets or remove existing ones by URL to maintain your digital asset library.
- **Targeting & Personalization** — Use user attributes and MongoDB-style queries to fetch specific content variants.

### How it works

1. Subscribe to this server
2. Enter your Builder.io Public Key (and Private Key for write access)
3. Start managing your digital experience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — query and update CMS content directly from your IDE without switching to the Builder dashboard
- **Content Managers** — automate bulk updates or content migrations using natural language instructions
- **Marketing Teams** — quickly inspect content targeting and pre-rendered HTML outputs for SEO checks


## Available Tools
- **admin_graphql**: Requires Private API Key.

Execute an Admin API GraphQL query/mutation
- **create_content**: Requires Private API Key.

Create a new content entry
- **delete_asset_by_url**: Delete an asset by its URL
- **delete_content**: Requires Private API Key.

Delete a content entry
- **get_content**: Get content from a Builder.io model
- **get_html**: Get pre-rendered HTML for a Builder.io model
- **query_graphql**: Query Builder.io content using GraphQL
- **update_content**: Requires Private API Key.

Update an existing content entry
- **upload_asset**: Requires Private API Key.

Upload an asset (image, video, document)


## Installation & Usage

To install and use the **Builder.io (Visual CMS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/builderio-visual-cms](https://vinkius.com/mcp/builderio-visual-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
