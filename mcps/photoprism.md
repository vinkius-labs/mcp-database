# PhotoPrism MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/photoprism)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/photoprism-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/photoprism-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search, browse, and manage your PhotoPrism media library — find photos by metadata, retrieve thumbnails, and stream videos via AI.

## Description
Connect your self-hosted **PhotoPrism** instance to any AI agent to interact with your personal media collection through natural language.

### What you can do

- **Advanced Search** — Query your library using keywords, colors, or dates with the `search_photos` tool.
- **Visual Previews** — Generate direct URLs for thumbnails in various sizes using `get_thumbnail_url`.
- **Video Streaming** — Access streaming links for your stored videos with `get_video_url`.
- **OAuth Management** — Handle authentication tokens and user information securely with `create_oauth_token` and `get_oauth_userinfo`.

### How it works

1. Subscribe to this server
2. Enter your PhotoPrism URL and API Token
3. Start searching and viewing your media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Photography Enthusiasts** — Quickly find specific shots without manual scrolling through thousands of files
- **Self-Hosters** — Integrate your private cloud with your favorite AI tools for a seamless media experience
- **Content Creators** — Retrieve assets from your library directly within your coding or writing workflow


## Available Tools
- **create_oauth_token**: Create an OAuth2 token
- **get_oauth_authorize**: Get OAuth2 Authorization
- **get_oauth_userinfo**: Get OAuth2 UserInfo
- **get_thumbnail_url**: Get a thumbnail image URL for a photo
- **get_video_url**: Get a video streaming URL
- **revoke_oauth_token**: Revoke an OAuth2 token
- **search_photos**: Search for photos in PhotoPrism


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PhotoPrism** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for photos of 'mountains' taken in 2023."

**🤖 AI Agent:**
> I found 5 photos of mountains from 2023. Here are the details for the most recent ones...

---

**👤 You:**
> "Get a high-resolution thumbnail for the photo with hash 7af8b9c0."

**🤖 AI Agent:**
> I've generated the URL for the 1920px thumbnail of that photo: [URL]

---

**👤 You:**
> "Show me my PhotoPrism account information."

**🤖 AI Agent:**
> Retrieving user info... Your account is registered as 'Admin' with the email 'admin@example.com'.


## Installation & Usage

To install and use the **PhotoPrism** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/photoprism](https://vinkius.com/mcp/photoprism)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
