# Brightcove MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brightcove)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage your video library via Brightcove Video Cloud — list videos, manage playlists, and monitor performance directly from any AI agent.

## Description
Connect your **Brightcove Video Cloud** account to any AI agent and orchestrate your video management, publishing, and analytics workflows through natural conversation.

### What you can do

- **Video Oversight** — List all videos in your library, search by tags or metadata, and retrieve detailed technical specifications.
- **Playlist Management** — Create, update, and manage playlists to organize your content for different platforms.
- **Metadata Control** — Update video names, descriptions, and states (active/inactive) directly from your workspace.
- **Content Organization** — Access and list folders to verify how your assets are structured.
- **Library Insights** — Retrieve total video counts and monitor the status of individual media assets.

### How it works

1. Subscribe to this server
2. Enter your Brightcove Account ID, Client ID, and Client Secret
3. Start managing your video assets from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — quickly check if a video is active or find specific assets without manual dashboard searches.
- **Video Producers** — retrieve metadata and técnicos details for production reports straight from their editor.
- **Developers** — verify API integrations and asset processing using natural language.


## Available Tools (10)
- **create_playlist**: Create a new playlist
- **delete_video**: Delete a video permanently
- **get_folder_videos**: List videos within a specific folder
- **get_playlist**: Get details of a specific playlist
- **get_video_count**: Get total number of videos in the account
- **get_video**: Get details of a specific video
- **list_folders**: List all video folders
- **list_playlists**: List all playlists
- **list_videos**: List all videos in the account
- **update_video**: Update metadata for a video


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brightcove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 videos added to my Brightcove account."

**🤖 AI Agent:**
> I've retrieved your recent videos. You have 5 new entries, including 'Product Demo V2' (ID: vid_1) and 'CEO Keynote' (ID: vid_2). Both are currently active.

---

**👤 You:**
> "Show the playlists I have configured."

**🤖 AI Agent:**
> Retrieving playlists... You have 3 active playlists: 'Marketing Highlights', 'Training Series', and 'Social Media Clips'. Which one would you like to see the videos for?

---

**👤 You:**
> "Find all videos tagged with 'tutorial'."

**🤖 AI Agent:**
> I found 8 videos tagged with 'tutorial'. Notable titles include 'Getting Started Guide', 'Advanced Features', and 'API Integration Walkthrough'.


## ❓ FAQ

**Q: Can I check if a video has been processed and is active?**
Yes! Use the `get_video` tool with the Video ID. Your agent will fetch the current state, showing if it is 'ACTIVE', 'INACTIVE', or still being processed.

**Q: How do I list all the videos with a specific tag?**
Simply ask the agent to `list_videos` and provide a search query like `tags:summer`. It will retrieve all matching media assets from your library.

**Q: Does the integration allow creating a new playlist?**
Yes. Use the `create_playlist` action and provide a name and type (e.g., EXPLICIT or SMART). You can then organize your videos into this new collection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brightcove](https://vinkius.com/mcp/brightcove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brightcove** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brightcove` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brightcove** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brightcove": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
