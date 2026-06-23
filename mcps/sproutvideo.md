# SproutVideo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sproutvideo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate video hosting and management via SproutVideo — manage videos, playlists, and analytics directly from any AI agent.

## Description
Connect your **SproutVideo** account to any AI agent and simplify your video hosting and content management through natural conversation.

### What you can do

- **Video Management** — List all hosted videos, retrieve detailed metadata, and monitor playback stats and plays
- **Playlist Control** — Query and manage video playlists to organize your content delivery
- **Metadata Automation** — Update video titles, descriptions, and tags programmatically directly from your agent
- **Cleanup & Maintenance** — Delete old or redundant videos and manage your storage usage
- **Operational Insights** — Query video tags to understand your library structure and content distribution

### How it works

1. Subscribe to this server
2. Enter your SproutVideo API Key from your account settings
3. Start managing your video library from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **create_playlist**: Create a new video playlist
- **get_account**: Get account information and usage
- **get_playlist**: Get details for a specific playlist
- **get_video_analytics**: Get analytics for a specific video
- **list_folders**: List all video folders
- **delete_video**: Delete a video
- **get_video_details**: Get details for a specific video
- **list_playlists**: List video playlists
- **list_video_tags**: List video tags
- **list_videos**: List SproutVideo videos
- **update_video_metadata**: Update video details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SproutVideo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all videos in SproutVideo."

**🤖 AI Agent:**
> I've retrieved your video library. You have 20 videos, including 'Product Demo 2024' (Duration: 120s) and 'Customer Success Story'.

---

**👤 You:**
> "Show me the video engagement analytics for all published videos with viewer retention data."

**🤖 AI Agent:**
> 45 published videos analyzed. Total plays: 23,400 this month. Total watch time: 1,234 hours. Average engagement: 67%. Top 5 by plays: "Product Demo 2025" (4,560 plays, 78% engagement, avg 4:23 watch time), "Getting Started Tutorial" (3,200 plays, 82%), "Customer Success Story" (2,100 plays, 71%), "Feature Walkthrough" (1,890 plays, 64%), "CEO Keynote" (1,456 plays, 55%). Retention analysis: 89% watch past 25%, 67% past 50%, 45% past 75%, 34% complete. Drop-off hotspots: intro screens (first 10 seconds). Bandwidth: 890 GB served.

---

**👤 You:**
> "Create a new playlist called Product Tutorials and add the top 5 most viewed tutorial videos."

**🤖 AI Agent:**
> Playlist created: "Product Tutorials". 5 videos added by view count: 1) "Getting Started Tutorial" (3,200 plays, 12 min). 2) "Feature Walkthrough" (1,890 plays, 8 min). 3) "Advanced Configuration" (1,234 plays, 15 min). 4) "API Integration Guide" (987 plays, 20 min). 5) "Mobile App Setup" (756 plays, 6 min). Total playlist duration: 61 minutes. Privacy: public (embeddable). Custom thumbnail generated from first video. Embed code and share link ready. SEO metadata: title and description auto-populated. Player: branded with company colors.


## ❓ FAQ

**Q: Can I list all my hosted videos using my AI agent?**
Yes! Use the `list_videos` tool to retrieve a comprehensive list of all videos currently hosted in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sproutvideo](https://vinkius.com/mcp/sproutvideo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SproutVideo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sproutvideo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SproutVideo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sproutvideo": {
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
