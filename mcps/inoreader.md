# Inoreader MCP Server

Follow hundreds of news sources and blogs with a powerful RSS reader that filters, organizes, and prioritizes content for you.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/inoreader)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Inoreader** account to any AI agent and transform how you monitor news, blogs, and social feeds through natural language control.

### What you can do

- **Feed Management** — List all your subscriptions and quickly add new RSS/Atom feeds by URL.
- **Content Extraction** — Fetch article contents from specific feeds, folders, or system streams with advanced filtering.
- **Organization** — List, create, rename, and delete tags or folders to keep your information architecture clean.
- **Engagement** — Star important articles, mark items as read, or batch-clear entire streams instantly.
- **Unread Monitoring** — Get real-time summaries of unread counts across all your categorized content.

### How it works

1. Subscribe to this server
2. Enter your Inoreader Access Token (found in your developer preferences)
3. Start querying and organizing your knowledge base from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Analysts** — aggregate intelligence from hundreds of sources and filter for specific keywords using AI.
- **Content Creators** — monitor industry trends and save inspiration directly to tagged folders without leaving your workspace.
- **Information Junkies** — keep your 'Unread' counts at zero by letting your AI assistant help you prioritize what truly matters.


## Available Tools
- **delete_tag**: Articles will remain but the organizational label is removed.

Delete a tag or folder
- **edit_tag**: Use "user/-/state/com.google/starred" to star/unstar an item.

Add or remove tags from articles (e.g., Starred)
- **get_unread_counts**: Get the number of unread items per feed/folder
- **get_user_info**: Get Inoreader user information
- **list_stream_contents**: Use "user/-/state/com.google/reading-list" for all items.

Get articles for a specific feed, folder, or tag
- **list_subscriptions**: List all user subscriptions (feeds)
- **list_tags**: List all user tags and folders
- **mark_all_as_read**: Mark all items in a stream as read
- **quick_add_subscription**: Subscribe to a new feed by URL
- **rename_tag**: Rename an existing tag or folder


## Installation & Usage

To install and use the **Inoreader** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inoreader](https://vinkius.com/mcp/inoreader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
