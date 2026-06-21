# Vimeo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vimeo-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vimeo-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vimeo-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage your Vimeo video library, search for content, and update video metadata directly from your AI agent.

## Description
Connect your **Vimeo** account to any AI agent to take full control of your video hosting and content management workflows through natural conversation.

### What you can do

- **Video Management** — Retrieve metadata, update titles/descriptions, and delete videos using specific IDs.
- **Search & Discovery** — Search for videos across the entire Vimeo platform or list videos from specific users, channels, or groups.
- **User Insights** — Access profile information for yourself or other users, including follower lists and albums.
- **Content Organization** — List and inspect albums, channels, and groups to understand how content is categorized.
- **Upload Preparation** — Create video upload tickets to streamline the process of adding new content to your library.

### How it works

1. Subscribe to this server
2. Enter your Vimeo Personal Access Token
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — quickly update video descriptions and privacy settings without leaving your workflow.
- **Marketing Teams** — search for brand assets and organize videos into albums via simple commands.
- **Developers** — inspect video metadata and user profiles directly from your coding environment.


## Available Tools
- **create_video_upload**: Create a video upload ticket
- **delete_video**: Delete a video
- **get_channel**: Get a specific channel
- **get_group**: Get a specific group
- **get_me**: Get the authenticated user profile
- **get_user**: Get a specific user profile
- **get_video**: Retrieve metadata for a specific video
- **list_my_videos**: List all videos belonging to the authenticated user
- **list_user_albums**: List a user albums (showcases)
- **list_user_followers**: List a user followers
- **list_user_videos**: Get a list of videos uploaded by a user
- **search_videos**: Search for videos on Vimeo
- **update_video**: Update video metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vimeo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent videos on Vimeo."

**🤖 AI Agent:**
> I've retrieved your latest uploads. You have 3 recent videos: 'Product Demo' (ID: 88231), 'Team Sync' (ID: 88245), and 'Tutorial Part 1' (ID: 88250). Would you like to see the details for any of these?

---

**👤 You:**
> "Search for videos about 'artificial intelligence' on Vimeo."

**🤖 AI Agent:**
> Searching Vimeo... I found several videos. The top results include 'AI Revolution 2024' and 'Understanding Neural Networks'. Should I provide more info on these?

---

**👤 You:**
> "Update the description of video 88231 to 'Updated product walkthrough'."

**🤖 AI Agent:**
> The video metadata has been updated successfully. Video ID 88231 now has the description: 'Updated product walkthrough'.


## Installation & Usage

To install and use the **Vimeo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vimeo-alternative](https://vinkius.com/mcp/vimeo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
