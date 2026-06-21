# Tumblr MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tumblr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tumblr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tumblr-mcp)
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


## Installation & Usage

To install and use the **Tumblr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tumblr](https://vinkius.com/mcp/tumblr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
