# Dailymotion MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dailymotion-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dailymotion-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dailymotion-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Dailymotion account — audit videos, playlists, and followers via AI.

## Description
Empower your AI agent to orchestrate your entire video ecosystem on **Dailymotion**, the innovative video sharing platform. By connecting Dailymotion to your agent, you transform complex asset management into a natural conversation. Your agent can instantly list your videos, audit playlist organization, and retrieve follower stats without you ever touching a dashboard. Whether you are a professional creator or a media brand, your agent acts as a real-time video operator, ensuring your content is always organized and your audience reach is monitored.

### What you can do

- **Video Auditing** — List all videos in your account and retrieve detailed metadata, including view counts and statuses.
- **Playlist Oversight** — Browse your playlists to maintain a clear view of your content categorization and sequencing.
- **Community Management** — List your followers and following lists to stay on top of your audience growth.
- **Video Governance** — Update video titles, descriptions, and autonomously delete items when they are no longer needed.
- **Search Intelligence** — Query public videos across Dailymotion to find relevant community content or inspiration.

### How it works

1. Subscribe to this server
2. Enter your Dailymotion Access Token
3. Start managing your video assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Creators** — monitor upload statuses and engagement metrics straight from your creation workflow.
- **Media Managers** — verify if new videos have been correctly categorized into playlists.
- **Account Admins** — perform rapid audits of video libraries and manage channel growth without manual logins.
- **Operations Leads** — automate video querying to orchestrate cross-functional content teams smoothly.


## Available Tools
- **delete_video**: Delete a video from Dailymotion
- **get_me**: Get authenticated user info from Dailymotion
- **get_video**: Get details for a specific video
- **list_followers**: List followers for a user
- **list_following**: List following for a user
- **list_playlists**: List playlists for a user
- **list_videos**: List videos for a user
- **search_videos**: Search for public videos on Dailymotion
- **update_video**: Update video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dailymotion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 videos in my Dailymotion account."

**🤖 AI Agent:**
> I've retrieved your recent videos. You have 5 files, including 'Spring Launch' and 'Interview V1'. Would you like the view counts for any of them?

---

**👤 You:**
> "Show me my Dailymotion playlists."

**🤖 AI Agent:**
> You have 3 playlists in your account: 'Promos', 'Demos', and 'Tutorials'. I can list the videos inside any of these playlists for you.

---

**👤 You:**
> "How many followers do I have on Dailymotion?"

**🤖 AI Agent:**
> Checking your audience... You currently have 150 followers. I can list the most recent ones for you if you'd like.


## Installation & Usage

To install and use the **Dailymotion** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailymotion-alternative](https://vinkius.com/mcp/dailymotion-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
