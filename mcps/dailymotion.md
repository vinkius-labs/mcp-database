# Dailymotion MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dailymotion)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dailymotion-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dailymotion-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage video hosting via Dailymotion — upload and publish videos, track view counts, manage playlists, and search public content directly from any AI agent.

## Description
Connect your **Dailymotion** account to any AI agent and take full control of your enterprise video hosting and content delivery workflows through natural conversation.

### What you can do

- **Video Orchestration** — List and retrieve your uploaded videos including detailed metadata: titles, channels, durations, and views_total
- **Public Content Discovery** — Search the global Dailymotion library by keyword to identify trending topics and public video payloads limitlessly
- **Asset Mutation** — Safely update video metadata by patching titles, descriptions, and tags, or permanently remove videos from your channel
- **Streamlined Uploads** — Retrieve temporary upload endpoints and publish hosted URLs directly to generate new video nodes natively from the chat
- **Playlist & Channel Oversight** — Manage custom playlists and list available content channels to verify categorical mappings and organizational boundaries
- **Identity Mapping** — Retrieve account-specific properties including total video counts and unified view telemetry tied to your authenticated profile

### How it works

1. Subscribe to this server
2. Enter your Dailymotion Access Token (obtained via OAuth flow in Dailymotion Studio)
3. Start managing your video content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Marketers** — upload and publish videos or update metadata without leaving the workspace
- **Video Producers** — monitor view telemetry and manage playlists across multiple channels using natural language
- **Developers** — test and debug Dailymotion API integrations and upload pipelines through the chat
- **Social Media Managers** — search for public content and audit channel performance in real-time


## Available Tools
- **list_videos**: List your uploaded Dailymotion videos. Returns video IDs, titles, channels, durations, view counts, and thumbnail URLs
- **get_video**: Get full details of a Dailymotion video. Returns title, description, channel, tags, duration, views, and stream URLs
- **search_videos**: Search all public Dailymotion videos by keyword. Returns matching videos with metadata
- **update_video**: g. title=New Title&tags=cat,funny).

Update video metadata on Dailymotion. Modify title, description, tags, channel, or published status
- **delete_video**: Delete a Dailymotion video permanently
- **get_upload_url**: Get a temporary upload URL from Dailymotion. Used as the first step in the upload flow
- **publish_video**: g. shortfilms, music), and comma-separated tags.

Publish a video to Dailymotion. Creates a new video entry from a previously uploaded file
- **get_user**: Get your Dailymotion account info. Returns username, email, total videos, and total views
- **list_playlists**: List your Dailymotion playlists. Returns playlist IDs, names, and video counts
- **list_channels**: List Dailymotion content channels. Returns channel IDs, names, and descriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dailymotion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 uploaded videos"

**🤖 AI Agent:**
> I found 5 recent videos on your channel. The latest is 'Product Launch 2024' (Views: 1,200). Others include 'API Tutorial' and 'Office Tour'. Would you like to see the full metadata for any of these?

---

**👤 You:**
> "Search for public videos about 'SpaceX Starship'"

**🤖 AI Agent:**
> Searching Dailymotion... I found several videos about 'SpaceX Starship'. The top results include 'Starship Flight 3 Highlights' and 'SpaceX Mars Mission Update'. Which one would you like to explore?

---

**👤 You:**
> "Change the title of video 'x8abc12' to 'Updated Tutorial'"

**🤖 AI Agent:**
> Title updated! Video 'x8abc12' is now named 'Updated Tutorial' on your Dailymotion channel. The changes are live and visible to your viewers.


## Installation & Usage

To install and use the **Dailymotion** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailymotion](https://vinkius.com/mcp/dailymotion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
