# Hashnode MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hashnode)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hashnode-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hashnode-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Hashnode blog directly from your AI agent — fetch user profiles, read publication posts, and publish or update content.

## Description
Connect your **Hashnode** account to any AI agent to streamline your technical writing and blogging workflow. This MCP server allows you to interact with the Hashnode GraphQL API through natural language.

### What you can do

- **User Profiles** — Retrieve detailed information about any Hashnode user by their handle using `get_user`.
- **Publication Management** — List all posts from a specific publication using its domain or hostname with `get_publication_posts`.
- **Content Retrieval** — Fetch full post content and metadata using slugs and hostnames via `get_post`.
- **Publishing** — Create and publish new blog posts with Markdown support and custom tags using `create_post` directly from your conversation.
- **Editing** — Update existing posts, titles, and content with `update_post` without leaving your AI interface.

### How it works

1. Subscribe to this server
2. Enter your Hashnode Personal Access Token
3. Start managing your technical blog from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Writers** — Draft and publish articles directly from your AI-assisted writing environment.
- **Developers** — Share knowledge and updates on your Hashnode blog without switching contexts.
- **Content Managers** — Monitor publication feeds and update existing posts efficiently.


## Available Tools
- **create_post**: Publish a new post to a publication
- **get_post**: Get a single post by its slug
- **get_publication_posts**: Get a list of posts from a specific publication
- **get_user**: Get details about a specific Hashnode user
- **update_post**: Modify an existing post


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hashnode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get details for Hashnode user 'johndoe'."

**🤖 AI Agent:**
> I've retrieved the profile for 'johndoe'. They are a Technical Writer with 1,200 followers and their blog is located at johndoe.hashnode.dev.

---

**👤 You:**
> "List all posts from the publication 'blog.hashnode.com'."

**🤖 AI Agent:**
> I found 10 recent posts on 'blog.hashnode.com'. The latest titles include 'Announcing New Features' and 'Markdown Guide for Developers'. Would you like to read the content of any of these?

---

**👤 You:**
> "Create a new post in publication '642f...' titled 'My MCP Guide' with content '# Introduction...'."

**🤖 AI Agent:**
> Successfully published your post 'My MCP Guide'! You can view it at your publication URL. The post ID is 65a2b...


## Installation & Usage

To install and use the **Hashnode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashnode](https://vinkius.com/mcp/hashnode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
