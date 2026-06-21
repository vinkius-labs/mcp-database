# Miniflux (RSS Reader) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miniflux-rss-reader)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your RSS feeds and read articles via Miniflux — discover feeds, list entries, and organize categories directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Miniflux (RSS Reader)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current RSS feeds and their IDs."

**🤖 AI Agent:**
> I've retrieved your feeds. You have 3 active subscriptions: 'TechCrunch' (ID: 12), 'Hacker News' (ID: 15), and 'Miniflux Blog' (ID: 20). Which one would you like to explore?

---

**👤 You:**
> "Find RSS feeds for the website https://miniflux.app."

**🤖 AI Agent:**
> Searching for feeds... I found one available subscription: 'Miniflux Blog' at https://miniflux.app/feed.xml. Would you like me to add it to your feeds?

---

**👤 You:**
> "Show me the latest 5 unread entries from feed ID 15."

**🤖 AI Agent:**
> Fetching unread entries for Hacker News (ID: 15)... Here are the latest 5: 'Show HN: MCP Server for Miniflux', 'New Rust Release', 'The Future of RSS', 'AI in 2024', and 'Web Standards Update'. Would you like to read the content of any of these?


## ❓ FAQ

**Q: Can I find RSS feeds from a website URL automatically?**
Yes! Use the `discover_subscriptions` tool with any website URL. The agent will scan the site and return all available RSS/Atom feed links found.

**Q: How do I mark all articles in a specific feed as read?**
Simply use the `mark_feed_as_read` action providing the `feed_id`. This will instantly update the status of all entries within that feed to 'read'.

**Q: Can I search for specific keywords across all my articles?**
Yes. Use the `list_entries` tool and provide a keyword in the `search` parameter. You can also filter by status (read/unread) or starred items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miniflux-rss-reader](https://vinkius.com/mcp/miniflux-rss-reader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Miniflux (RSS Reader)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `miniflux-rss-reader` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Miniflux (RSS Reader)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "miniflux-rss-reader": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
