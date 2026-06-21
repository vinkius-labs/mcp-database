# Vimeo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vimeo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vimeo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vimeo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Vimeo account — audit videos, folders, and showcases via AI.

## Description
Empower your AI agent to orchestrate your entire video ecosystem on **Vimeo**, the world's most innovative video platform. By connecting Vimeo to your agent, you transform complex asset management into a natural conversation. Your agent can instantly list your videos, audit project folders, and retrieve performance stats without you ever touching a dashboard. Whether you are a professional filmmaker or a corporate communications lead, your agent acts as a real-time video operator, ensuring your content is always organized and accessible.

### What you can do

- **Video Auditing** — List all videos in your account and retrieve detailed metadata, including duration, plays, and privacy settings.
- **Folder Oversight** — Browse your project folders to maintain a clear view of your content organization.
- **Showcase Management** — List all showcases (albums) and channels to monitor your public video distribution.
- **Video Governance** — Update video titles, descriptions, and autonomously delete items when they are no longer needed.
- **Search Intelligence** — Query public videos across Vimeo to find inspiration or relevant community content.

### How it works

1. Subscribe to this server
2. Enter your Vimeo Access Token
3. Start managing your video assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Professionals** — monitor upload statuses and metadata straight from your production workflow.
- **Content Marketers** — verify if new videos have been correctly added to showcases and folders.
- **Account Admins** — perform rapid audits of video libraries and clean up old content without manual logins.
- **Operations Leads** — automate video querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **delete_video**: Delete a video from Vimeo
- **get_me**: Get authenticated user info from Vimeo
- **get_video**: Get details for a specific video
- **list_channels**: List channels followed by a user
- **list_folders**: List folders (projects) for a user
- **list_groups**: List groups followed by a user
- **list_showcases**: List showcases (albums) for a user
- **list_videos**: List videos for a user
- **search_videos**: Search for public videos on Vimeo
- **update_video**: Update video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vimeo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 videos in Vimeo."

**🤖 AI Agent:**
> I've retrieved your recent videos. You have 5 files, including 'Client Feedback V2' and 'Final Master'. Would you like the full metadata for any of them?

---

**👤 You:**
> "Show me my Vimeo project folders."

**🤖 AI Agent:**
> You have 3 projects in Vimeo: 'Corporate', 'Ads 2024', and 'Social Media'. I can list the videos inside any of these folders for you.

---

**👤 You:**
> "Search for public videos about 'Artificial Intelligence'."

**🤖 AI Agent:**
> I've found several public videos about 'Artificial Intelligence'. The top matches include 'The Future of AI' and 'Deep Learning Explained'. Would you like the links to watch them?


## Installation & Usage

To install and use the **Vimeo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vimeo](https://vinkius.com/mcp/vimeo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
