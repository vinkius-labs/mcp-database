# Dailymotion MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dailymotion-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dailymotion-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dailymotion-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage your Dailymotion video library — upload content, edit metadata, customize players, and access advanced reporting directly via AI.

## Description
Connect your **Dailymotion** account to any AI agent and take full control of your video hosting and distribution workflows through natural conversation.

### What you can do

- **Video Uploads** — Generate secure upload URLs and publish new videos to specific channels with full metadata control.
- **Content Management** — Search, list, and filter your video library. Update titles, descriptions, tags, and privacy settings instantly.
- **Streaming & Delivery** — Retrieve direct HLS or MP4 stream URLs for integration into other platforms or for deep inspection.
- **Custom Players** — Create and manage customized video players for specific profiles using the Partner API.
- **Advanced Reporting** — Execute complex GraphQL queries against the Reporting API to track performance and metrics.

### How it works

1. Subscribe to this server
2. Enter your Dailymotion Access Token
3. Start managing your video content from Claude, Cursor, or any MCP-compatible client

No more navigating complex API dashboards to update a video tag or find a stream link. Your AI acts as your dedicated media manager.

### Who is this for?

- **Content Creators** — quickly update video details and manage uploads without leaving your workflow.
- **Developers** — fetch stream URLs and player configurations directly into your code editor.
- **Media Managers** — orchestrate large video libraries and pull performance reports using natural language.


## Available Tools
- **create_player**: Create a new video player
- **create_video**: Create or publish a new video
- **edit_video**: Edit video metadata
- **get_partner_upload_url**: Requires private API key/token.

Get a partner upload URL for a video file
- **get_upload_url**: Get a public upload URL for a video file
- **get_video_stream**: Generate stream or download URLs for a video
- **list_videos**: List and search videos
- **reporting_graphql**: g., askPartnerReportFile).

Query the Reporting API via GraphQL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dailymotion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the latest 5 videos about 'artificial intelligence' on Dailymotion."

**🤖 AI Agent:**
> I've searched Dailymotion for 'artificial intelligence'. Here are the 5 most recent results, including 'AI Revolution 2024' and 'Future of Robotics'. Would you like the stream URLs for any of these?

---

**👤 You:**
> "Update the title of video x82j1k9 to 'Product Demo v2' and add 'tutorial' to the tags."

**🤖 AI Agent:**
> I've successfully updated video x82j1k9. The title is now 'Product Demo v2' and the tags have been updated to include 'tutorial'.

---

**👤 You:**
> "Get me an upload URL so I can publish a new video."

**🤖 AI Agent:**
> I've generated a secure upload URL for you. You can upload your file to: [Upload URL]. Once finished, give me the file URL and I'll use `create_video` to publish it.


## Installation & Usage

To install and use the **Dailymotion** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailymotion-extended](https://vinkius.com/mcp/dailymotion-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
