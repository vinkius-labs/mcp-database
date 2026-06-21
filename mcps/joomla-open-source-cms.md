# Joomla (Open-Source CMS) MCP Server

Manage content via Joomla — list and create articles, manage categories and tags, and audit site menus.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/joomla-open-source-cms)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Joomla** site to any AI agent and take full control of your content management and digital publication lifecycle through natural conversation.

### What you can do

- **Article Orchestration** — List, retrieve, and create new content articles directly from your agent, including support for custom titles, aliases, and HTML introtext
- **Categorization & Taxonomy** — Manage global content categories and system tags to ensure your articles are accurately mapped and organized
- **Structural Audit** — Extract detailed information about site menus and menu items to understand your website's navigation hierarchy and layout
- **User Management** — List registered platform users and monitor roles to understand team distribution across your Joomla instance
- **Marketing & Banners** — Enumerate active advertising banners and tracking modules to monitor your site's promotional performance
- **Content Lifecycle** — Update or irreversibly delete specific CMS articles to maintain a fresh and optimized digital storefront

### How it works

1. Subscribe to this server
2. Enter your Joomla Base URL and API Token
3. Start managing your CMS from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Digital Content Editors** — publish and update articles quickly through natural conversation without logging into the Joomla administrator backend
- **Web Developers** — test API results and audit site structures through real-time REST queries directly from your workspace
- **Site Administrators** — monitor user activity, categories, and menu configurations across multiple Joomla projects efficiently


## Available Tools
- **create_cms_article**: Requires title, alias, category ID, and HTML introtext.

Create a new Joomla article
- **delete_cms_article**: Delete a Joomla article
- **get_article_details**: Get details for a specific Joomla article
- **list_site_articles**: You can optional pass query parameters like filter[state]=1.

List Joomla articles
- **list_active_banners**: List Joomla banners
- **list_global_categories**: List Joomla categories
- **list_site_menus**: List Joomla site menus
- **list_system_tags**: List Joomla tags
- **list_platform_users**: List Joomla users
- **patch_cms_article**: Update an existing Joomla article


## Installation & Usage

To install and use the **Joomla (Open-Source CMS)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/joomla-open-source-cms](https://vinkius.com/mcp/joomla-open-source-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
