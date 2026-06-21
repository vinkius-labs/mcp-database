# WordPress MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wordpress-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wordpress-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage posts, pages, and media on WordPress — the world's most popular open-source content management system.

## Description
Connect your **WordPress** site to any AI agent and take control of your content infrastructure through natural conversation.

### What you can do

- **Post Management** — List all blog articles, create new posts with HTML/Block content, and update metadata or status (draft, publish, private)
- **Static Pages** — Browse and manage hierarchical content like 'About Us' or 'Contact' pages directly from your agent
- **Media Library** — List all uploaded assets (images, documents) and retrieve their direct public URLs for content distribution
- **Taxonomy Auditing** — List and browse all categories and tags used across your site to ensure consistent content organization
- **User Discovery** — Retrieve a list of all registered site users and their associated numeric IDs for author attribution
- **Content Insights** — Get comprehensive details for specific posts, including full content, featured media, and technical status
- **Data Integrity** — Safely trash or permanently delete obsolete posts through simple chat commands

### How it works

1. Subscribe to this server
2. Enter your WordPress Base URL, Username, and Application Password
3. Start managing your content through Claude, Cursor, or any MCP-compatible client

No more manual logging into the WP-Admin dashboard to fix a typo. Your AI agent becomes your WordPress content editor.

### Who is this for?

- **Blogging Teams** — quickly draft and publish articles and manage post status through simple conversation
- **CMS Administrators** — audit site users, monitor categories, and manage media attachments without manual navigation
- **Marketing Managers** — verify publication status and retrieve media URLs for social sharing and campaigns
- **Web Developers** — test REST API responses and verify content structure for headless WordPress applications


## Available Tools
- **delete_cms_post**: Set force to true for permanent deletion, otherwise it goes to Trash.

Permanently deletes a WordPress post
- **create_cms_post**: Provide a title, content, and initial status (draft, publish, private).

Creates a new post in WordPress
- **get_post_details**: Retrieves details for a specific WordPress post
- **list_site_categories**: Lists all categories defined in WordPress
- **list_media_attachments**: Lists media files (images, documents) from the WordPress library
- **list_static_pages**: Lists static pages from the WordPress site
- **list_site_posts**: Supports standard WP query parameters like per_page and categories.

Lists posts from the WordPress site
- **list_site_tags**: Lists all tags used in the WordPress site
- **list_site_users**: Lists all registered WordPress users
- **update_cms_post**: Provide the post ID and a JSON object of fields to update.

Updates an existing WordPress post


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WordPress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 posts on my WordPress site."

**🤖 AI Agent:**
> I found your 5 most recent posts: 1. 'Welcome to 2026' (ID: 101, Status: publish), 2. 'New Product Features' (ID: 102, Status: draft), 3. 'Our Vision' (ID: 103, Status: publish), and 2 others. Which one would you like to see the details for?

---

**👤 You:**
> "Create a new draft post titled 'AI in Marketing' with content '<p>AI is changing everything...</p>'."

**🤖 AI Agent:**
> Success! I've created a new draft post titled 'AI in Marketing' (ID: 155). It is currently saved as a draft. Would you like me to add any tags or categories to it?

---

**👤 You:**
> "List all categories on my WordPress site."

**🤖 AI Agent:**
> I found 4 categories: 'News' (ID: 1), 'Tutorials' (ID: 2), 'Product Updates' (ID: 3), and 'Case Studies' (ID: 4). Would you like to see how many posts are assigned to each?


## Installation & Usage

To install and use the **WordPress** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress](https://vinkius.com/mcp/wordpress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
