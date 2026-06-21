# Inoreader MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inoreader)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/inoreader-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/inoreader-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Follow hundreds of news sources and blogs with a powerful RSS reader that filters, organizes, and prioritizes content for you.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inoreader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the latest news from my Tech folder?"

**🤖 AI Agent:**
> I've fetched the contents of your 'Tech' folder. Here are the top 3 stories: 'New AI Breakthrough' from TechCrunch, 'React 19 Released' from Dev.to, and 'The Future of Web3' from Wired. Would you like me to summarize any of these?

---

**👤 You:**
> "Find articles about 'SpaceX' that I haven't read yet."

**🤖 AI Agent:**
> Searching your unread reading list... I found 2 articles related to SpaceX: 'Starship Test Flight Update' and 'Falcon 9 Launch Schedule'. Both are marked as unread. Shall I open the description for the Starship flight?

---

**👤 You:**
> "Mark all articles in my 'Social Media' tag as read."

**🤖 AI Agent:**
> Processing batch update... Done! All articles within the 'Social Media' tag have been marked as read. Your unread count for this tag is now zero.


## Installation & Usage

To install and use the **Inoreader** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inoreader](https://vinkius.com/mcp/inoreader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
