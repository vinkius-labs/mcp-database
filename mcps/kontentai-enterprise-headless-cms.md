# Kontent.ai (Enterprise Headless CMS) MCP Server

Manage enterprise content via Kontent.ai — create items, publish language variants, and audit content types.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kontentai-enterprise-headless-cms)

## Overview
**Category:** collaboration
**Tools Count:** 10

## Description
Connect your **Kontent.ai** project to any AI agent and take full control of your enterprise-grade headless CMS and content orchestration through natural conversation.

### What you can do

- **Item Orchestration** — List and retrieve content item containers, and create or update top-level item shells defining types and codenames directly from your agent
- **Variant Management** — Update actual content fields (`elements`) for specific languages (e.g., English, Portuguese), moving variants into Draft status securely
- **Publishing Workflow** — Transition specific language variants from Draft to Published status to make content immediately live via Delivery APIs
- **Schema Introspection** — Discover and inspect Content Type definitions to understand available fields, scalar parameters, and required element blocks
- **Taxonomy & Tags** — Manage hierarchical taxonomy groups used to classify and filter your content assets for better organizational structure
- **Media Audit** — List uploaded media assets and document files to retrieve precise identifiers and cloud URLs for frontend delivery

### How it works

1. Subscribe to this server
2. Enter your Kontent.ai Environment ID and Management API Key
3. Start managing your content lifecycle from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Content Editors** — update and publish content variants quickly through natural conversation without logging into the Kontent.ai UI
- **Content Architects** — audit taxonomy trees and verify content type schemas across multiple environments and projects efficiently
- **Frontend Developers** — introspect content types and verify asset identifiers to ensure accurate mapping in your downstream applications


## Available Tools
- **get_item**: Retrieve metadata for a specific Kontent.ai item by codename
- **get_taxonomy**: Get details and nested terms for a specific Taxonomy group
- **get_content_type**: Retrieve the exact structural fields of a specific Content Type
- **list_assets**: List uploaded Media Assets and Document files
- **list_items**: ai project space.

List all content items in the Kontent.ai environment
- **list_taxonomies**: List all hierarchical Taxonomies (tags/categories)
- **list_content_types**: List all Content Type schemas registered in the environment
- **publish_variant**: Publish a specific language variant of an item to Delivery APIs
- **upsert_item**: Note: this does not update the language variant fields (the actual content text)—use upsert_language_variant for that.

Create or update a top-level content item container
- **upsert_language_variant**: g. `default`). This places the variant into Draft status.

Update the actual content fields of an item for a specific language


## Installation & Usage

To install and use the **Kontent.ai (Enterprise Headless CMS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kontentai-enterprise-headless-cms](https://vinkius.com/mcp/kontentai-enterprise-headless-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
