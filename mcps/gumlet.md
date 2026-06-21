# Gumlet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gumlet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Optimize images and stream video with automatic format conversion, lazy loading, and CDN delivery that loads pages faster.

## Description
Connect your **Gumlet** account to any AI agent and take full control of your video hosting and image optimization workflows through natural conversation.

### What you can do

- **Video Lifecycle** — Manage the complete video lifecycle from creating new uploads and retrieving metadata to monitoring transcoding status
- **Media Organization** — Create and manage collections/folders programmatically to maintain a structured media library
- **Visual Control** — Automate thumbnail updates by selecting specific video frames or time offsets for perfect visual representation
- **Optimization Insights** — Monitor real-time video analytics, viewing metrics, and bandwidth usage for every asset in your account
- **Image Source Management** — List and manage image optimization sources and organization users to ensure high-fidelity delivery

### How it works

1. Subscribe to this server
2. Retrieve your API Key from your Gumlet dashboard (Profile icon > API Key)
3. Start managing your video and image infrastructure from Claude, Cursor, or any MCP client

No more manual status checking or complex asset management through slow web dashboards. Your AI acts as your dedicated media infrastructure engineer.

### Who is this for?

- **Video Platform Developers** — automate asset ingestion and monitor transcoding progress through natural language
- **Digital Marketers** — retrieve engagement analytics and update video thumbnails across multiple collections
- **Content Managers** — organize large media libraries and manage team access to specific image sources


## Available Tools
- **create_video_upload**: Upload new video
- **create_collection**: Add new folder
- **delete_video**: Remove video asset
- **get_video_details**: Check video status
- **get_account_info**: Get profile details
- **get_video_analytics**: Check video stats
- **list_videos**: List video assets
- **list_video_collections**: List folders
- **list_image_sources**: List image optimized sources
- **list_org_users**: List team members
- **list_webhooks**: Get active webhooks
- **update_video_thumbnail**: Set thumbnail offset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gumlet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new video upload in collection 'col_123' titled 'Annual Report 2026'."

**🤖 AI Agent:**
> Upload initialized! I've created the asset 'Annual Report 2026' (ID: asset_987). You can now upload your file to the following URL: [upload_url]. I'll monitor the transcoding status for you.

---

**👤 You:**
> "Check the transcoding status of video 'asset_987'."

**🤖 AI Agent:**
> Checking asset_987... The video is currently 75% through transcoding. I'll alert you as soon as the HLS and DASH streams are ready for playback.

---

**👤 You:**
> "Show me the viewing stats for my latest product video."

**🤖 AI Agent:**
> Fetching analytics... Your latest video has 1,250 unique views and has consumed 45GB of bandwidth this month. Most viewers are based in North America and Europe.


## ❓ FAQ

**Q: How do I start a video upload?**
Use the `create_video_upload` tool, which will create the asset in your specified collection and provide a temporary `upload_url` for your file.

**Q: Can I update the thumbnail for a video already uploaded?**
Yes! The `update_video_thumbnail` tool allows you to specify a time offset in seconds. Gumlet will extract that specific frame and set it as the new thumbnail.

**Q: Does it support viewing stats and bandwidth usage?**
The `get_video_analytics` tool provides detailed viewing metrics and bandwidth consumption data for any video ID in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gumlet](https://vinkius.com/mcp/gumlet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gumlet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gumlet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gumlet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gumlet": {
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
