# PeerTube (YouTube Alternative) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/peertube-youtube-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/peertube-youtube-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/peertube-youtube-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Interact with decentralized PeerTube instances — manage video feeds, download content, and handle user registration via AI.

## Description
Connect your **PeerTube** instance to any AI agent to explore the decentralized video ecosystem. This server allows you to interact with the Fediverse's leading video platform through natural language.

### What you can do

- **Video Discovery** — Access public video feeds and comment streams in multiple formats (RSS, Atom, JSON, XML).
- **Content Retrieval** — Fetch public and private web videos, HLS playlists, and generate direct download links for offline viewing.
- **User Management** — Register new accounts on instances and manage OAuth 2.0 authentication tokens directly.
- **System Monitoring** — Track the status of background processing jobs for video transcoding and federation.
- **OAuth Integration** — Retrieve local client credentials to facilitate secure third-party application connections.

### How it works

1. Subscribe to this server
2. Enter your PeerTube Instance URL (e.g., `https://peertube.example.com`)
3. (Optional) Provide your Personal Access Token for private content and administrative tasks
4. Start querying videos and managing your instance from your favorite MCP client

### Who is this for?

- **Content Creators** — Monitor video processing jobs and manage feeds across the Fediverse.
- **Developers** — Test API integrations and retrieve OAuth credentials without manual terminal commands.
- **Privacy Enthusiasts** — Access decentralized video content through a secure, AI-driven interface.


## Available Tools
- **generate_video_download**: Generate video download
- **get_completed_jobs**: Requires authentication.

Get completed jobs
- **get_local_oauth_clients**: Get local OAuth clients
- **get_private_web_video**: Requires a videoFileToken.

Get private Web Video file
- **get_public_hls_playlist**: Get public HLS playlist file
- **get_public_web_video**: Get public Web Video file
- **get_user_token**: 0 access token.

Get user access token
- **get_video_comments_feed**: Get video comments feed
- **get_video_feeds**: Get video feeds
- **register_user**: Register a new user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PeerTube (YouTube Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve the local OAuth client credentials for this PeerTube instance."

**🤖 AI Agent:**
> I've retrieved the OAuth client details. The Client ID is `...` and the Client Secret is `...`. You can use these to request a user token.

---

**👤 You:**
> "Show me the latest video comments feed in JSON format."

**🤖 AI Agent:**
> Fetching the comments feed... I've found the latest comments in JSON format. Would you like me to summarize the most recent discussions?

---

**👤 You:**
> "Generate a download link for the video with ID 'a1b2c3d4'."

**🤖 AI Agent:**
> Processing request... I have generated a download link for video 'a1b2c3d4'. You can access the mp4 file here: [Link].


## Installation & Usage

To install and use the **PeerTube (YouTube Alternative)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/peertube-youtube-alternative](https://vinkius.com/mcp/peertube-youtube-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
