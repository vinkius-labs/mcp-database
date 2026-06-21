# PhotoPrism MCP Server

Search, browse, and manage your PhotoPrism media library — find photos by metadata, retrieve thumbnails, and stream videos via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/photoprism)

## Overview
**Category:** productivity
**Tools Count:** 7

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


## Installation & Usage

To install and use the **PhotoPrism** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/photoprism](https://vinkius.com/mcp/photoprism)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
