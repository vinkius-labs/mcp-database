# Tumblr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tumblr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Publish multimedia blog posts, follow creative communities, and engage with millions of users on the iconic blogging platform.

## Description
Connect your **Tumblr** account to any AI agent and simplify how you manage your blogs, discover trending content, and track social interactions through natural conversation.

### What you can do

- **Blog Insights** — Retrieve general metadata and avatar details for any Tumblr blog using its name or hostname.
- **Content Discovery** — List and search for the latest posts across the entire Tumblr platform matching specific tags.
- **Post Management** — List published posts from specific blogs, optionally filtering by type (text, photo, quote, etc.).
- **Individual Tracking** — Fetch complete data for specific posts to analyze engagement or content details.
- **Social Oversight** — Monitor your microblogging presence and discover new creators directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Tumblr API Consumer Key (found in your developer apps)
3. Start managing your social blogging from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators** — quickly retrieve post metadata and check blog avatars via simple AI commands.
- **Social Media Managers** — monitor trending tags and discover new content for curation directly from the workspace.
- **Data Analysts** — retrieve post histories and analyze engagement levels across different Tumblr blogs.


## Available Tools
- **get_blog_avatar**: Get the avatar URL for a blog
- **get_blog_info**: g., "officialtumblr").

Get information about a Tumblr blog
- **get_post**: Get details for a specific post
- **list_blog_posts**: List posts for a specific blog
- **list_tagged_posts**: Search posts by tag


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tumblr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the latest posts tagged with 'illustration'."

**🤖 AI Agent:**
> I've retrieved the latest tagged posts. Here are some beautiful illustrations trending right now from creators across Tumblr. Would you like the details for any specific post?

---

**👤 You:**
> "List all photo posts from the blog 'officialtumblr'."

**🤖 AI Agent:**
> I've fetched the photo posts from 'officialtumblr'. You have 5 recent images including anniversary graphics and community features. Shall I retrieve the full description for the latest one?

---

**👤 You:**
> "Get information about the blog 'staff'."

**🤖 AI Agent:**
> Fetching blog info... The 'staff' blog is the official Tumblr internal blog. It has over 1M followers and focuses on product updates and platform news. Would you like to see their latest posts?


## ❓ FAQ

**Q: Can I search for posts matching a specific tag across Tumblr?**
Yes! Use the `list_tagged_posts` tool and provide your tag. Your agent will retrieve the latest posts from across the platform that use that specific tag.

**Q: How do I see the posts from a specific blog like 'officialtumblr'?**
Run the `list_blog_posts` query with the blog name. You can optionally filter by type (e.g., 'photo' or 'quote') to see only the content you're interested in.

**Q: Is it possible to retrieve the avatar URL of a blog via AI?**
Absolutely. Use the `get_blog_avatar` tool and provide the blog name. You can also specify an optional size to get the image URL that best fits your needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tumblr](https://vinkius.com/mcp/tumblr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tumblr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tumblr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tumblr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tumblr": {
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
