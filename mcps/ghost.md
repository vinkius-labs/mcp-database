# Ghost MCP Server

Manage blog posts, track authors, and oversee static pages via AI agents with Ghost CMS.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ghost)

## Overview
**Category:** productivity
**Tools Count:** 11

## Description
Connect your **Ghost** publication to any AI agent to automate your content management workflows through the Model Context Protocol (MCP). Ghost is a powerful headless Node.js CMS tailored for modern publishing. This MCP server enables you to retrieve published posts, manage taxonomy tags, and fetch site configurations directly through natural conversation using the Ghost Content API.

### Key Features

- **Content Discovery** — List all published blog posts and static pages, retrieving detailed HTML content and metadata.
- **Taxonomy Oversight** — Retrieve and list all categorization tags to understand your content architecture.
- **Author Management** — Fetch profile details for active writers and contributors across the publication.
- **Site Configuration** — Access global settings, routing rules, and title schemas programmatically.
- **Subscription Insights** — Retrieve active membership tiers to understand paywall rules and pricing layers.
- **Real-time Synchronization** — Keep your headless CMS content accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Ghost Base URL and Content API Key (found in Integrations)
3. Start managing your publication from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Managers** — quickly retrieve published post data or list active authors without manual dashboard navigation.
- **Frontend Developers** — automate the retrieval of taxonomy tags and site configuration via simple AI commands.
- **Editorial Leads** — get a real-time overview of the static pages and subscription tiers active on the site.


## Available Tools
- **verify_api_connection**: Check connection
- **get_post_by_slug**: Get post details
- **get_author_details**: Get author profile
- **get_page_by_slug**: Get page details
- **get_site_settings**: Get site settings
- **get_tag_details**: Get tag metadata
- **list_subscription_tiers**: List subscription tiers
- **list_blog_authors**: List authors
- **list_static_pages**: List static pages
- **list_published_posts**: List published posts
- **list_content_tags**: List categories/tags


## Installation & Usage

To install and use the **Ghost** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ghost](https://vinkius.com/mcp/ghost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
