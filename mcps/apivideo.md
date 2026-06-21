# api.video MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apivideo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apivideo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apivideo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Host, encode, and stream video content with a developer-first API that handles everything from upload to playback.

## Description
Connect your **api.video** account to any AI agent and take full control of your professional video hosting infrastructure and automated media workflows through natural conversation.

### What you can do

- **Video Orchestration** — List and manage your entire high-fidelity video library programmatically, or create new video objects to prepare for uploads in real-time
- **Asset Intelligence** — Retrieve detailed high-fidelity status and direct asset URLs for players, thumbnails, and navigation markers (chapters) directly through your agent
- **Deep Analytics Tracking** — Monitor performance metrics like total plays and impressions using high-fidelity aggregation tools to coordinate your content strategy
- **Multilingual Captions** — Access and manage subtitle tracks across multiple languages to maintain a perfectly coordinated global viewer experience
- **Infrastructure Monitoring** — Access your directory of custom player themes and store-level metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Production API Key** from your api.video dashboard (API Keys section)
3. Start orchestrating your video content and performance from Claude, Cursor, or any MCP client

No more manual toggling between video dashboards or digging through complex embed settings. Your AI acts as your dedicated video engineer and media architect.

### Who is this for?

- **Content Creators** — instantly retrieve player links and update video metadata using natural language commands
- **Product Managers** — monitor video performance and track feature walkthrough engagement without leaving your creative workspace
- **Developers** — integrate high-speed cloud-based video management into custom application workflows through simple AI queries


## Available Tools
- **create_video_object**: Set title and description here.

Initialize a new video
- **delete_video**: video.

Permanently delete a video
- **get_video_analytics**: Retrieve performance metrics
- **get_video_details**: Get metadata for a video
- **list_video_captions**: List captions for a video
- **list_video_chapters**: List chapters for a video
- **list_player_themes**: List custom player themes
- **list_videos**: Supports filtering by title or tags.

List your api.video videos
- **update_video_details**: Modify video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **api.video** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 videos in my api.video account."

**🤖 AI Agent:**
> I've retrieved your video library. You have 5 recent uploads, including 'Project Alpha Demo' (ID: vi123) and 'Onboarding Tutorial'. Would you like the detailed high-fidelity status for any of these?

---

**👤 You:**
> "Show the play count analytics for all videos this month."

**🤖 AI Agent:**
> Accessing media intelligence... This month, your videos have reached a total of 12,450 plays. Your top performing asset is 'Product Feature v2' with 5,200 impressions. Shall I retrieve the high-fidelity hourly breakdown?

---

**👤 You:**
> "Get the player link and captions for video ID 'vi123'."

**🤖 AI Agent:**
> Asset orchestrated! For video vi123, the high-fidelity player URL is [url]. I've also identified 2 available caption tracks: English and French. Need help updating the video high-fidelity metadata?


## Installation & Usage

To install and use the **api.video** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apivideo](https://vinkius.com/mcp/apivideo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
