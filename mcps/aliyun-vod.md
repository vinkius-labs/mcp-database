# Aliyun VOD / 阿里云视频点播 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aliyun-vod)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Alibaba Cloud's professional video pipeline — manage media, retrieve play URLs, and audit transcode templates via AI.

## Description
Empower your AI agent to orchestrate your video infrastructure and digital asset management with **Aliyun VOD** (视频点播), the premier media processing platform in China. By connecting Aliyun VOD to your agent, you transform complex media listing, playback authorization, and upload management into a natural conversation. Your agent can instantly retrieve detailed video metadata, generate authorized play URLs, search through massive video libraries, and manage media categories without you ever needing to navigate the comprehensive Aliyun Console. Whether you are conducting a digital content audit or coordinating a video distribution workflow, your agent acts as a real-time media operations specialist, providing accurate and fast results from a single, authorized source.

### What you can do

- **Media Orchestration** — List stored videos, retrieve technical metadata, and permanently delete obsolete media assets.
- **Playback Management** — Automatically generate secure play URLs and retrieve definition details for any VideoId.
- **Content Discovery** — Search your media library using advanced matching and filter by categories.
- **Upload Automation** — Initialize video uploads by retrieving UploadAuth and UploadAddress tokens directly through the agent.
- **Template Auditing** — List available transcode template groups to ensure consistent video processing standards.

### How it works

1. Subscribe to this server
2. Enter your Aliyun AccessKey ID and AccessKey Secret
3. Start managing your video infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Media Operations Teams** — automate routine metadata updates and monitor library health through natural language.
- **Product Managers** — audit video assets and verify playback availability directly from your AI-powered workspace.
- **Developers** — integrate professional-grade media pipelines into your AI-driven daily routines.
- **Aliyun Power Users** — integrate your existing VOD workflows into your AI-driven daily routines.


## Available Tools (8)
- **create_upload_auth**: Get upload credentials
- **delete_media**: Delete VOD video
- **get_media_metadata**: Get video info
- **get_playback_info**: Get play URLs
- **list_categories**: List media categories
- **list_media**: List VOD media
- **refresh_upload_auth**: Refresh upload token
- **search_vod_media**: Search media library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aliyun VOD / 阿里云视频点播** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent 10 videos in my Aliyun VOD library."

**🤖 AI Agent:**
> I've retrieved your recent media list. I found 10 videos, including 'Main_Event_Recap' (VideoId: `88210934`) and 'Product_Demo_v2'. Would you like me to get the authorized play URLs for any of these?

---

**👤 You:**
> "Get the technical metadata and playback info for video '88210934'."

**🤖 AI Agent:**
> I've retrieved the details for video `88210934`. It has a duration of 120s and is currently in 'Normal' status. I've also generated authorized play URLs for SD, HD, and Full HD definitions. Should I check which transcode template was used for this file?

---

**👤 You:**
> "Search for videos matching 'Tutorial' and show their categories."

**🤖 AI Agent:**
> I've performed a search for 'Tutorial'. I found 5 matching videos. Most of them are classified under the 'Education' category (ID: `1024`). Would you like me to list all available categories in your VOD project to help organize your library better?


## ❓ FAQ

**Q: How do I find my Aliyun AccessKey ID and Secret?**
Log in to the [Alibaba Cloud Console](https://usercenter.console.aliyun.com/), navigate to [AccessKey Management] to find or create your unique ID and Secret.

**Q: What is a VideoId?**
A VideoId is the unique identifier for a video file in the Aliyun VOD system. It is assigned when a video is created or uploaded and is required for all video-specific operations like metadata retrieval or playback info.

**Q: Does this server handle authentication signatures?**
Yes! The server automatically calculates the required Aliyun RPC signature (HMAC-SHA1) for every request using your provided AccessKey Secret, ensuring secure authorized communication with the Aliyun VOD gateway.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aliyun-vod](https://vinkius.com/mcp/aliyun-vod)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aliyun VOD / 阿里云视频点播** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aliyun-vod` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aliyun VOD / 阿里云视频点播** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aliyun-vod": {
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
