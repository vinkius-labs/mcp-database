# Miniflux (RSS Reader) MCP Server

Manage your RSS feeds and read articles via Miniflux — discover feeds, list entries, and organize categories directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/miniflux-rss-reader)

## Overview
**Category:** productivity
**Tools Count:** 46

## Description
Connect your **Miniflux** instance to any AI agent and transform how you consume information. Manage your RSS feeds, read articles, and organize your knowledge base through natural conversation.

### What you can do

- **Feed Discovery & Management** — Discover RSS feeds from any URL and manage your subscriptions effortlessly with tools like `discover_subscriptions` and `create_feed`.
- **Article Reading** — List entries, fetch full content, and mark items as read or unread using `list_entries` and `fetch_entry_content`.
- **Organization** — Categorize feeds and use bookmarks to save important information with `list_categories` and `toggle_entry_bookmark`.
- **System Control** — Export/Import OPML files and manage your user profile and API keys directly.

### How it works

1. Subscribe to this server
2. Enter your Miniflux Instance URL and API Key
3. Start reading and managing your news from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — aggregate sources and query specific topics across all subscriptions without leaving your research environment.
- **Developers** — stay updated with technical blogs and releases directly from your IDE.
- **Content Curators** — quickly filter, search, and bookmark relevant articles for newsletters or social media.


## Available Tools
- **create_api_key**: Create a new API key
- **create_category**: Create a category
- **create_feed**: Create a new feed
- **create_user**: Create a user (Admin only)
- **delete_api_key**: Delete an API key
- **delete_category**: Delete a category
- **delete_feed**: Remove a feed
- **delete_user**: Delete a user (Admin only)
- **discover_subscriptions**: Discover subscriptions from a URL
- **export_opml**: OPML Export
- **fetch_entry_content**: Fetch original article content
- **flush_history**: Flush history
- **get_entry**: Get a single entry
- **get_feed_counters**: Fetch unread and read counters
- **get_feed_icon**: Get feed icon by feed ID
- **get_feed**: Get a specific feed
- **get_icon**: Get feed icon by icon ID
- **get_integrations_status**: Check if any third-party integrations are enabled
- **get_me**: Get current user information
- **get_user**: Get a specific user (Admin only)
- **get_version**: Get application version and build info
- **healthcheck**: Healthcheck (checks DB)
- **import_entry**: Import an entry manually
- **import_opml**: OPML Import
- **list_api_keys**: List API keys
- **list_categories**: Get all categories
- **list_category_entries**: Get entries for a specific category
- **list_entries**: Get entries with filters
- **list_feed_entries**: Get entries for a specific feed
- **list_feeds**: Get all feeds
- **list_users**: Get all users (Admin only)
- **liveness**: Liveness probe
- **mark_category_as_read**: Mark all entries in a category as read
- **mark_feed_as_read**: Mark all entries of a feed as read
- **mark_user_as_read**: Mark all entries for a user as read
- **readiness**: Readiness probe
- **refresh_all_feeds**: Refresh all feeds (background)
- **refresh_category**: Refresh all feeds in a category
- **refresh_feed**: Refresh a specific feed (synchronous)
- **save_entry**: Save entry to third-party services
- **toggle_entry_bookmark**: Toggle entry bookmark (starred)
- **update_category**: Update a category
- **update_entries_status**: Update status of multiple entries (e.g., mark as read)
- **update_entry**: Update entry title or content
- **update_feed**: Update a feed
- **update_user**: Update a user (Admin only)


## Installation & Usage

To install and use the **Miniflux (RSS Reader)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miniflux-rss-reader](https://vinkius.com/mcp/miniflux-rss-reader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
