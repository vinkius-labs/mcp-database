# Cockpit (Self-hosted Headless CMS API) MCP Server

Manage your self-hosted Cockpit CMS content, assets, and menus directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cockpit-self-hosted-headless-cms-api)

## Overview
**Category:** developer-tools
**Tools Count:** 17

## Description
Connect your **Cockpit CMS** instance to any AI agent and take full control of your headless content infrastructure through natural conversation.

### What you can do

- **Content Management** — List, fetch, create, update, and delete items from any content collection using Mongo-style filters.
- **Asset Handling** — Retrieve file metadata and generate processed thumbnails or resized images on the fly.
- **Navigation & Menus** — Access and manage menus and page structures via the Pages addon integration.
- **Batch Operations** — Fetch data from multiple content models in a single request for high-performance workflows.
- **Localization** — Support for multi-language content retrieval and localized project management.

### How it works

1. Subscribe to this server
2. Enter your Cockpit Instance URL and API Key
3. Start managing your CMS content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — Update blog posts, products, or FAQs without logging into the CMS dashboard.
- **Developers** — Query content structures and asset metadata directly from your IDE while coding.
- **Marketing Teams** — Quickly retrieve localized content and assets for multi-channel campaigns.


## Available Tools
- **batch_content_items**: Batch request content from multiple models
- **create_or_update_content_item**: If an _id is provided in the data, it updates the existing item.

Create or update a content item
- **delete_content_item**: Delete a content item by ID
- **get_asset_image**: Generate thumbnails or resized images
- **get_asset**: Get asset metadata by ID
- **get_content_item**: Fetch a single content item by ID
- **get_lokalize_project_locale**: Get translations for a specific locale in a Lokalize project
- **get_lokalize_project**: Get all translations for a Lokalize project
- **get_menu**: Get a specific menu by name
- **get_page_by_route**: Fetch a page by its route
- **get_sitemap**: Get the complete sitemap
- **list_content_items**: Supports filtering, sorting, and pagination.

Fetch a list of items from a Cockpit content collection
- **list_menus**: List all menus
- **list_pages**: List all pages
- **list_routes**: Get a lightweight list of all routes and slugs
- **search_detektivo**: Search within a specific Detektivo index
- **submit_inbox**: Submit form data to an Inbox


## Installation & Usage

To install and use the **Cockpit (Self-hosted Headless CMS API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cockpit-self-hosted-headless-cms-api](https://vinkius.com/mcp/cockpit-self-hosted-headless-cms-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
