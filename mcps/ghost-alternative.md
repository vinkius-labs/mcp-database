# Ghost MCP Server

Publish and monetize your content with a modern headless CMS built for newsletters, memberships, and independent creators.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ghost-alternative)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Ghost** publishing account to any AI agent and take full control of your content management and membership workflows through natural conversation.

### What you can do

- **Content Orchestration** — List and manage all blog posts (published, draft, scheduled) and retrieve detailed HTML content and metadata programmatically
- **Member Intelligence** — Query your subscriber directory and retrieve detailed profiles, including join dates and membership tiers to monitor audience growth
- **Site Navigation** — List and oversee static site pages (About, Contact) and manage content tags to maintain a perfectly organized site taxonomy
- **Publishing Control** — Create new posts or drafts and update publishing statuses directly through your agent to streamline your editorial pipeline
- **Site Visibility** — Retrieve general site settings, newsletter configurations, and active membership offers using natural language commands

### How it works

1. Subscribe to this server
2. Retrieve your **Admin API Key** and **Admin Domain** from Ghost (Settings > Integrations > Custom Integration)
3. Start managing your digital publication from Claude, Cursor, or any MCP client

No more manual dashboard navigation to check post statuses or member counts. Your AI acts as your dedicated content strategist and site manager.

### Who is this for?

- **Content Managers** — instantly retrieve post details and manage drafts without opening the Ghost admin panel
- **Digital Publishers** — monitor membership tiers and verify newsletter configurations using natural language
- **Marketing Teams** — automate site settings querying to orchestrate cross-platform content strategies


## Available Tools
- **create_post**: Requires a title and supports optional HTML content. The post is created as a "draft" by default but can be set to "published" immediately.

Create a new Ghost post or draft
- **get_post_details**: Essential for reviewing the full content of an article.

Get details for a specific post
- **get_site_settings**: Essential for verifying site identity.

Get Ghost site settings and configuration
- **list_members**: Includes emails, status, and join dates.

List all site members
- **list_newsletters**: Newsletters are used to send content updates to members.

List all configured newsletters
- **list_offers**: List active membership offers
- **list_pages**: g., About, Contact) defined on the Ghost site. Pages are similar to posts but used for non-blog content.

List all static site pages
- **list_posts**: Includes basic metadata and post IDs for detailed retrieval.

List all Ghost blog posts
- **list_tags**: Useful for organizing and filtering posts.

List all content tags
- **list_membership_tiers**: g., Free, Premium) available on the site. Useful for understanding the subscription structure.

List membership tiers and plans


## Installation & Usage

To install and use the **Ghost** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ghost-alternative](https://vinkius.com/mcp/ghost-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
