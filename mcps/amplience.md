# Amplience MCP Server

Connect your Amplience CMS to your AI agent — query hubs, pull content, edit schemas, and deploy live items easily via chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amplience)

## Overview
**Category:** ecommerce
**Tools Count:** 10

## Description
Link your **Amplience** headless CMS to any intelligent AI agent to completely rethink how you handle your enterprise content architecture, deploying components natively through standard conversation.

### What you can do

- **Discover Asset Hierarchies** — Freely list top-level Hubs, target specific Repositories, and fetch internal Folders to help your AI inherently understand where every graphic and article lives.
- **Content Retrieval** — Paginate through dynamic content items, safely extracting complete metadata alongside current active schemas and validation rules.
- **Edit & Create Structure** — Give the agent full permission to push correctly strictly-typed JSON payloads back into the system, generating or modifying blog entries and product metadata.
- **Manage Deployments** — Permanently execute deletions (if revision locks permit) or instruct the system to fire a specific content configuration directly over to the edge delivery API to hit the live website.

### How it works

1. Enable the connector within your environment.
2. Submit your exact Amplience Hub Name alongside a Personal Access Token.
3. Oversee and iterate your site configurations natively using Claude, Cursor, or other MCP counterparts.

### Who is this for?

- **E-commerce Managers** — ask the agent to rapidly locate the Black Friday banner content configuration block and update the live URL paths seamlessly.
- **Frontend Developers** — have your IDE agent read the precise output validation structure of an Amplience schema and automatically scaffold the corresponding React/Vue TypeScript interface in your project.
- **Content Marketers** — command your agent to create a brand new draft for a promotional blog post, pre-populating fields utilizing your CRM's specific SEO guidelines.


## Available Tools
- **create_content_item**: Create a new structured content item adhering to a schema inside a folder
- **delete_content_item**: Requires version validation before deletion.

Permanently delete a content item from the repository database
- **get_content_item**: Retrieve a specific content item configuration and its schema revision lock
- **list_content_items**: Retrieve paginated content items from a specific repository
- **get_delivery_content**: Retrieve the exact structural matching verifying Delivery CDN blocks
- **list_folders**: List all folders organizing content in a given repository
- **list_hubs**: Essential for retrieving the active workspace.

List all accessible Amplience Hubs (environments)
- **list_repositories**: List all content repositories within a specific Hub
- **publish_content_item**: Publish a specific content item version to the live delivery CDN
- **update_content_item**: Update an existing content item data structure matching its current schema


## Installation & Usage

To install and use the **Amplience** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplience](https://vinkius.com/mcp/amplience)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
