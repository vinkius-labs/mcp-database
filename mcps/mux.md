# Mux MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mux)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mux-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mux-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage video assets and live streams via Mux — create assets and track performance directly from your AI agent.

## Description
Connect your **Mux Video** account to your AI agent and take full control of your video infrastructure and streaming workflows through natural conversation.

### What you can do

- **Asset Management** — List all video assets and get real-time status updates, durations, and playback IDs.
- **Asset Creation** — Create new video assets instantly by providing a public URL to your source file.
- **Live Streaming** — Access and monitor your live stream configurations and their current status.
- **Direct Uploads** — Create secure upload sessions for uploading video files directly.
- **Video Analytics** — Get recent video view metrics to track your content's reach.
- **Deep Inspection** — Fetch complete metadata for specific assets or live streams using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Mux Token ID and Token Secret
3. Start managing your video content from Claude, Cursor, or any MCP client

### Who is this for?

- **Video Developers** — quickly check if an asset has finished processing without opening the Mux dashboard.
- **Content Platforms** — automate the creation of new assets directly from your communication or development tools.
- **Broadcast Teams** — monitor live stream health and configurations in real-time.


## Available Tools
- **create_asset**: Create a new video asset
- **create_direct_upload**: Create a direct upload session
- **create_live_stream**: Create a new live stream
- **delete_asset**: Delete a video asset
- **delete_live_stream**: Delete a live stream
- **get_asset**: Get specific asset details
- **get_live_stream**: Get specific live stream details
- **get_recent_views**: Get recent video views analytics
- **list_assets**: List Mux video assets
- **list_direct_uploads**: List direct video uploads
- **list_live_streams**: List Mux live streams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mux** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my video assets and show their status."

**🤖 AI Agent:**
> I've retrieved your video assets. You have 12 assets, including 'asset-123' (Status: ready) and 'asset-456' (Status: processing). Shall I check if 'asset-456' is finished now?

---

**👤 You:**
> "Create a new video asset from https://example.com/video.mp4."

**🤖 AI Agent:**
> I've initiated the creation of a new video asset from the URL provided. The new Asset ID is 'new-asset-789' and its current status is 'preparing'. I'll let you know when it's ready for playback.

---

**👤 You:**
> "Check recent views for my videos."

**🤖 AI Agent:**
> Fetching recent analytics... You had 156 views in the last 15 minutes, with a 98% player success rate. Shall I breakdown the views by country?


## Installation & Usage

To install and use the **Mux** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mux](https://vinkius.com/mcp/mux)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
