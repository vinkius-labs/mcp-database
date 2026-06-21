# Dev.to (Forem Developer Community API) MCP Server

Manage your Dev.to presence — publish articles, track engagement, and interact with the developer community directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/devto-forem-developer-community-api)

## Overview
**Category:** developer-tools
**Tools Count:** 36

## Description
Connect your **Dev.to** (Forem) account to your AI agent to streamline your technical writing and community management. This server provides full access to the Forem API, allowing you to handle content and community interactions without leaving your workspace.

### What you can do

- **Article Management** — Create, update, and list your articles. Manage drafts and published content with tools like `create_article` and `list_my_all_articles`.
- **Community Interaction** — Retrieve and manage comments using `list_comments`, and engage with content via `create_reaction`.
- **User & Org Insights** — Fetch profile data for users and organizations, list followers, and manage your reading list.
- **Content Discovery** — Search for articles by tags, popularity, or specific users using `list_articles` and `get_article_by_path`.
- **Admin & Moderation** — For authorized users, manage pages, display ads, and user status within a Forem instance.

### How it works

1. Subscribe to this server
2. Enter your Dev.to API Key (found in your account settings)
3. Start publishing and managing your developer community content from Claude, Cursor, or any MCP client

### Who is this for?

- **Technical Writers** — Draft and publish articles directly from your markdown editor.
- **Developer Advocates** — Monitor community feedback and respond to comments efficiently.
- **Content Marketers** — Track article performance and manage cross-posted content.


## Available Tools
- **create_article**: Create a new article
- **create_display_ad**: Create a display ad
- **create_page**: Create a page
- **create_reaction**: Create a reaction
- **delete_page**: Delete page by ID
- **get_article_by_path**: Get article by username and slug
- **get_article**: Get article by ID
- **get_comment**: Get comment by ID
- **get_display_ad**: Get display ad by ID
- **get_me**: Get authenticated user profile
- **get_organization**: Get organization by username
- **get_page**: Get page by ID
- **get_profile_image**: Get profile image by username
- **get_user**: Get user by ID
- **list_articles**: List published articles
- **list_comments**: List comments
- **list_display_ads**: List display ads
- **list_followed_tags**: List followed tags for the authenticated user
- **list_followers**: List followers of the authenticated user
- **list_my_all_articles**: List all authenticated user's articles (published and unpublished)
- **list_my_articles**: List authenticated user's articles
- **list_my_published_articles**: List authenticated user's published articles
- **list_my_unpublished_articles**: List authenticated user's unpublished articles
- **list_organization_articles**: List organization's articles
- **list_organization_users**: List organization's users
- **list_pages**: List pages
- **list_podcast_episodes**: List published podcast episodes
- **list_reading_list**: List authenticated user's reading list
- **list_tags**: List tags used in the community
- **list_videos**: List articles with videos
- **suspend_user**: Suspend a user (Admin)
- **toggle_reaction**: Toggle a reaction
- **unpublish_article**: Unpublish an article (Admin/Moderator)
- **update_article**: Update article by ID
- **update_display_ad**: Update display ad by ID
- **update_page**: Update page by ID


## Installation & Usage

To install and use the **Dev.to (Forem Developer Community API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devto-forem-developer-community-api](https://vinkius.com/mcp/devto-forem-developer-community-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
