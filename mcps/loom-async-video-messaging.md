# Loom (Async Video Messaging) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loom-async-video-messaging)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage video messages via Loom — retrieve metadata, handle timeline comments, and track viewer analytics.

## Description
Connect your **Loom** account to any AI agent and take full control of your asynchronous video communication and screencast management through natural conversation.

### What you can do

- **Video Orchestration** — List all accessible workspace videos and retrieve detailed metadata including titles, durations, and exact permalinks directly from your agent
- **Timeline Engagement** — Read, add, or delete threaded comments on any video timeline to maintain high-touch communication without opening the browser
- **Viewer Analytics** — Extract detailed session telemetry to understand exact watch segments and viewership numbers for your shared content
- **Digital Delivery** — Generate precise ephemeral MP4 download endpoints to retrieve raw video files physically, bypassing internal UI locking
- **Organization Control** — Update video titles and properties in real-time, or relocate specific screencasts into target workspace folders for better library management
- **Cleanup Operations** — Irreversibly delete specific screencast videos to maintain a clean and optimized video workspace

### How it works

1. Subscribe to this server
2. Enter your Loom API Token
3. Start managing your video library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Teams** — track customer engagement with shared video solutions and respond to timeline queries through natural conversation
- **Product Managers** — audit viewer sessions for feature walkthroughs and organize feedback comments across multiple project videos
- **Remote Leaders** — manage team video updates and monitor viewership analytics to ensure critical information is being consumed effectively


## Available Tools
- **list_videos**: List all Loom videos
- **get_video**: Get video details
- **delete_video**: This action cannot be undone.

Delete a video
- **update_video**: Update video title
- **get_transcript**: Get video transcript
- **list_folders**: List workspace folders
- **list_workspace_members**: List workspace members
- **get_video_analytics**: Get video analytics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loom (Async Video Messaging)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 videos in my Loom workspace"

**🤖 AI Agent:**
> I've retrieved the 5 most recent videos. Highlights include 'Product Demo Q1' (ID: vid-123), 'Bug Report: Login Flow' (ID: vid-456), and 'Quick Update' (ID: vid-789). Would you like to see the viewership analytics for the product demo?

---

**👤 You:**
> "Show me the comments for video ID 'vid-123'"

**🤖 AI Agent:**
> I've found 3 comments on 'Product Demo Q1': 1) Sarah: 'Great overview, can we add more detail on the API?', 2) Alex: 'Looks good!', 3) Mark: 'When is this launching?'. Would you like me to draft a reply to Sarah?

---

**👤 You:**
> "Get the download link for video ID 'vid-456'"

**🤖 AI Agent:**
> Generating download URL… Done. You can download the raw MP4 file for 'Bug Report: Login Flow' here: [pre-signed-s3-url]. Note that this link is ephemeral and will expire in 1 hour.


## ❓ FAQ

**Q: Can I see who watched my video using my agent?**
Yes. Use the `list_viewer_sessions` tool with a specific Video ID. Your agent will retrieve the viewing telemetry, allowing you to see exactly how many times the video was watched and which specific segments were most engaging.

**Q: How do I download a raw MP4 file of a Loom video through a conversation?**
The `create_download_url` tool forces the backend to allocate an ephemeral S3 pre-signed URL. Your agent will provide this link, which allows you to stream or download the raw bytes of your video directly.

**Q: Can my agent respond to comments on my video timeline?**
Absolutely. Use the `add_timeline_comment` tool to post threaded messages directly to the video. Your agent can help you maintain community interaction by drafting and sending replies through natural conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loom-async-video-messaging](https://vinkius.com/mcp/loom-async-video-messaging)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loom (Async Video Messaging)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `loom-async-video-messaging` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loom (Async Video Messaging)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loom-async-video-messaging": {
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
