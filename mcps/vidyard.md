# Vidyard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vidyard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage video assets, players, and hosting on Vidyard — the leading video messaging platform for business.

## Description
Connect your **Vidyard** account to any AI agent and manage your business video library through natural conversation.

### What you can do

- **Video Library** — List all video assets stored in your Vidyard dashboard and retrieve unique video IDs
- **Metadata & Details** — Get technical metadata for any video including length, encoding status, and descriptions
- **Player Management** — Create, update, and manage video players (facades) to customize how your content is embedded
- **Video Organization** — Attach videos to specific players and organize your content for different marketing or sales needs
- **Direct Stream Access** — Retrieve direct stream URLs and raw MP4 download links for various video qualities (480p, 720p, etc.)
- **Asset Management** — Rename players or permanently delete video assets and player containers from your dashboard

### How it works

1. Subscribe to this server
2. Enter your Vidyard API Token
3. Start managing your video library through Claude, Cursor, or any MCP-compatible client

No more manual browsing through complex video dashboards. Your AI agent becomes your video asset manager.

### Who is this for?

- **Marketing Teams** — organize video players for different campaigns and retrieve embed codes through chat
- **Sales Professionals** — quickly find and share specific videos or product demos with prospects
- **Content Creators** — manage video assets, check encoding status, and retrieve source files for distribution
- **Support Engineers** — find relevant tutorial videos and manage player branding for knowledge base articles


## Available Tools (10)
- **create_empty_player**: Creates a new, empty video player container
- **delete_video_player**: Note that the original video assets are not deleted.

Permanently deletes a video player
- **delete_video_asset**: This action is irreversible.

Permanently deletes a video asset from Vidyard
- **get_video_source_files**: Retrieves direct stream URLs for various video qualities (480p, 720p, etc.)
- **get_player_details**: Retrieves details for a specific video player
- **get_video_details**: Retrieves technical metadata for a specific video asset
- **list_video_players**: Lists all configured video players (facades) in the account
- **list_videos**: Lists all video assets stored in the Vidyard dashboard
- **attach_video_to_player**: Requires both player ID and video ID.

Adds a video asset into a specific player container
- **update_player_name**: Updates the display name or title of an existing player


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vidyard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my videos in Vidyard."

**🤖 AI Agent:**
> I found 8 videos in your library. The most recent ones are 'Q4 Product Update' (ID: vy-123), 'Sales Training 101' (ID: vy-456), and 'Customer Interview' (ID: vy-789). Would you like the full details for any of these?

---

**👤 You:**
> "Get the direct download links for the 'Product Demo' video."

**🤖 AI Agent:**
> Here are the direct stream and download links for 'Product Demo': 1080p (MP4: https://vidyard.com/stream/...), 720p (MP4: https://vidyard.com/stream/...), and 480p (MP4: https://vidyard.com/stream/...).

---

**👤 You:**
> "Create a new player called 'Website Homepage' and attach my latest video to it."

**🤖 AI Agent:**
> Success! I've created the player 'Website Homepage' (ID: pl-999) and attached the video 'Company Vision 2026' (ID: vy-888) to it. The player is now ready for embedding.


## ❓ FAQ

**Q: Can I get direct download links for my videos through the agent?**
Yes. The `get_video_source_files` tool allows your agent to retrieve direct MP4 download links and stream URLs for different qualities (like 720p or 1080p), making it easy to share raw files or use them in other applications.

**Q: How do I add a video to a specific player?**
Use the `attach_video_to_player` tool. You'll need to provide the `player_id` and the `video_id`. Your agent can help you find these IDs by listing your players and videos first.

**Q: Can I create new video players through conversation?**
Absolutely. The `create_empty_player` tool lets you provision a new player container with a descriptive name. Once created, you can attach videos to it and manage its settings directly through your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vidyard](https://vinkius.com/mcp/vidyard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vidyard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vidyard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vidyard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vidyard": {
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
