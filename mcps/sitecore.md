# Sitecore MCP Server

Manage your Sitecore CMS via AI agents — create, search, and update content items, templates, layouts, and workflows directly from your chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sitecore)

## Overview
**Category:** industry-titans
**Tools Count:** 9

## Description
Connect your **Sitecore** instance to any AI agent and take full control of your enterprise CMS through natural conversation. Execute headless content operations without navigating the complex Sitecore Content Editor.

### What you can do

- **Item Management** — Retrieve, create, update, and delete Sitecore items using their path or unique ID
- **Content Search** — Search deeply across your content tree using keywords, templates, and dates
- **Site navigation** — List item children to traverse the content tree hierarchy natively
- **Templates & Layouts** — List available templates and retrieve presentation/layout details (renderings and placeholders) for specific pages
- **Workflows** — Check the current workflow state of any item (e.g., Draft, Review, Published)

### How it works

1. Subscribe to this server
2. Provide your Sitecore Base URL and your Services Client API Key (Item ID)
3. Start managing your digital experience platform from Claude, Cursor, or any MCP-compatible client

No more context-switching between your editor and the Sitecore backend. Your AI agent becomes your CMS copilot.

### Who is this for?

- **Content Authors** — quickly update field values across multiple pages and see their workflow states without opening the Sitecore client
- **Marketers** — rapid searches to find legacy content items or verify if specific personalized components are in the right layout
- **Developers** — automate the creation of test items and query complex Sitecore trees while coding your front-end headless applications


## Available Tools
- **create_content_item**: Requires parent ID, item name, and template ID.

Creates a new item in the Sitecore content tree
- **delete_content_item**: This action is irreversible.

Permanently deletes a Sitecore item
- **get_item_details**: Retrieves details for a specific Sitecore item
- **get_item_layout**: Retrieves the layout or presentation details for an item
- **get_workflow_state**: Retrieves the current workflow state of an item
- **list_item_children**: Lists the immediate children of a specific item
- **list_content_templates**: g., "Page", "Article") are available for creating new items.

Lists available content templates
- **search_content**: Useful for broad discovery across the CMS.

Searches for content items in Sitecore
- **update_content_item**: Provide a JSON string of field name/value pairs.

Updates the fields of an existing Sitecore item


## Installation & Usage

To install and use the **Sitecore** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sitecore](https://vinkius.com/mcp/sitecore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
