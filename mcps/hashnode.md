# Hashnode MCP Server

Manage your Hashnode blog directly from your AI agent — fetch user profiles, read publication posts, and publish or update content.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hashnode)

## Overview
**Category:** productivity
**Tools Count:** 5

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


## Installation & Usage

To install and use the **Hashnode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hashnode](https://vinkius.com/mcp/hashnode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
