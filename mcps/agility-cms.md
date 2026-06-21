# Agility CMS MCP Server

Manage and query your Agility CMS content through AI — navigate sitemaps, search lists, and fetch layouts.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/agility-cms)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Agility CMS** instance to your AI agent and turn it into the ultimate Headless CMS assistant. Skip manual API queries and interact directly with your content architecture using natural language.

### What you can do

- **Sitemap & Routing** — Retrieve nested sitemap trees or flat router architectures to understand how your channels are structured
- **Content Lists** — Search, list, and count items across specific CMS references like articles, authors, or products
- **Page Layouts** — Fetch exact page modules, UI components mapping, and structural layout definitions using Page IDs
- **Content Operations** — Read full content payloads for individual items and synchronize granular CMS updates over time
- **Media Galleries** — Fetch specific media asset groups and tracking galleries for imagery

### How it works

1. Subscribe to this server
2. Provide your Agility GUID, target Locale, and API Key
3. Let your agent seamlessly query documents, pages, and components via Claude or Cursor

### Who is this for?

- **Frontend Developers** — get an instant breakdown of page modules and sitemaps while building frontends
- **Content Managers** — audit content lists, search for specific entries, and check page structures directly
- **SEO Specialists** — analyze the flat site router graph natively to map out content opportunities


## Available Tools
- **get_page_layout**: Retrieve the layout and structural modules of a single Page
- **get_site_flat_router**: Retrieve the exact flat list of all CMS routes/pages
- **count_reference_items**: Get the total size/count of items in a specific Reference List
- **get_media_gallery**: Retrieve a specific media gallery mapping containing photos
- **get_single_item**: g., an article body) knowing its numeric content ID.

Retrieve a single Agility CMS content item by its ID
- **get_site_tree**: Requires the target channel name.

Retrieve the nested sitemap architecture of a digital channel
- **list_content_items**: g. blog posts, articles, authors). The items are retrieved from the Headless CMS environment.

List content items from an Agility CMS Reference list
- **search_content_reference**: Search for specific keywords inside a Content Reference List
- **sync_incremental_items**: Start with 0 for full backup.

Get incrementally updated items since the last sync token
- **sync_incremental_pages**: Start with 0 for a full fetch.

Get incrementally updated pages since the last sync token


## Installation & Usage

To install and use the **Agility CMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agility-cms](https://vinkius.com/mcp/agility-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
