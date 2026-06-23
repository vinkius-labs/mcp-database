# api.video MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apivideo-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate video workflows via api.video — upload, stream, and analyze video content directly from any AI agent.

## Description
Connect your **api.video** account to any AI agent and take full control of your video infrastructure through natural conversation.

### What you can do

- **Video Management** — Create video containers, upload from URLs, and manage your entire library with full CRUD capabilities.
- **Live Streaming** — Create, update, and manage live streams, including starting and completing broadcast sessions.
- **Advanced Analytics** — Retrieve detailed metrics, breakdowns, and timeseries data to understand your video performance.
- **Player & Customization** — Create custom players, manage watermarks, and handle thumbnails with precise timecodes.
- **Content Enrichment** — Manage captions, chapters, and AI-generated summaries to make your videos more accessible and searchable.
- **Webhooks & Automation** — Set up webhooks to react to video events and manage upload tokens for secure client-side ingestion.

### How it works

1. Subscribe to this server
2. Enter your api.video API Key
3. Start managing your video assets from Claude, Cursor, or any MCP-compatible client

No more jumping between API documentation and dashboards to manage your video pipeline. Your AI acts as a dedicated video engineer.

### Who is this for?

- **Developers** — integrate video features and check encoding statuses without leaving the code editor.
- **Content Managers** — organize video libraries, update metadata, and manage captions through simple chat commands.
- **Data Analysts** — quickly pull viewership metrics and performance breakdowns for reporting.


## Available Tools (49)
- **complete_live_stream**: Stop a running live stream
- **create_live_stream**: Create a live stream object
- **create_player**: Create and customize a player theme
- **create_summary**: Generate a summary (abstract and takeaways) for a video
- **create_upload_token**: Generate a new delegated upload token
- **create_video**: Create a new video object (container)
- **create_webhook**: Subscribe to events via webhook
- **delete_caption**: Delete a caption
- **delete_chapter**: Delete a chapter
- **delete_live_stream**: Delete a live stream
- **delete_player_logo**: Remove the logo from a player theme
- **delete_player**: Delete a player theme
- **delete_summary**: Delete a summary
- **delete_upload_token**: Delete an upload token
- **delete_video**: Delete a video
- **delete_watermark**: Delete a watermark
- **delete_webhook**: Unsubscribe and delete a webhook
- **get_caption**: Retrieve a specific caption
- **get_chapter**: Retrieve a specific chapter
- **get_discarded_video**: Retrieve details of a discarded video
- **get_live_stream**: Retrieve live stream details
- **get_metrics_breakdown**: Get analytics metrics breakdown
- **get_metrics_timeseries**: Get analytics metrics time series
- **get_metrics**: Get aggregated analytics metrics
- **get_player**: Retrieve player theme details
- **get_summary_source**: Retrieve summary text
- **get_upload_token**: Retrieve upload token details
- **get_video_status**: Check upload and encoding status of a video
- **get_video**: Retrieve video details
- **get_webhook**: Retrieve webhook details (includes signatureSecret)
- **list_captions**: List all captions for a video
- **list_chapters**: List all chapters for a video
- **list_discarded_videos**: List discarded videos (if Video Restore is enabled)
- **list_live_streams**: List all live streams
- **list_players**: List player themes
- **list_summaries**: List all summaries
- **list_tags**: List all video tags used in the project and their video counts
- **list_upload_tokens**: List active upload tokens
- **list_videos**: video project.

List all video objects
- **list_watermarks**: List all watermarks
- **list_webhooks**: List configured webhooks
- **restore_discarded_video**: Restore a discarded video
- **update_caption_default**: Set a caption as default
- **update_live_stream**: Update live stream settings
- **update_player**: Update a player theme
- **update_summary_source**: Manually update summary content
- **update_thumbnail**: Set a thumbnail from a specific timecode
- **update_video**: Update video parameters
- **upload_video_source**: Ingest a video source from a URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **api.video** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the videos in my api.video account."

**🤖 AI Agent:**
> I've retrieved your video list. You have 12 videos. The most recent ones are 'Product Demo' (ID: vi4k0j...) and 'Customer Interview' (ID: vi2l9m...). Would you like details on any of these?

---

**👤 You:**
> "Check the encoding status for video vi4k0jv6psL."

**🤖 AI Agent:**
> The video 'Product Demo' (vi4k0jv6psL) is currently 100% encoded for HLS and 720p, 1080p qualities are ready. It is playable and ready for distribution.

---

**👤 You:**
> "Create a new live stream titled 'Q4 All Hands'."

**🤖 AI Agent:**
> Live stream 'Q4 All Hands' has been created successfully. Your Stream Key is '7f8e9a...' and the RTMP server is 'rtmp://broadcast.api.video/s'. You can start broadcasting whenever you're ready.


## ❓ FAQ

**Q: Can I check if a video has finished encoding and is ready to play?**
Yes! Use the `get_video_status` tool with the Video ID. It will return the ingestion and encoding status, letting you know exactly when the video is playable.

**Q: How do I upload a video file that is already hosted online?**
You can use the `upload_video_source` tool. Just provide the Video ID and the public URL of the source file, and api.video will ingest it automatically.

**Q: Is it possible to see how many people watched my videos yesterday?**
Absolutely. Use the `get_metrics` or `get_metrics_timeseries` tools to retrieve viewership data and performance analytics for your account or specific videos.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apivideo-alternative](https://vinkius.com/mcp/apivideo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **api.video** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apivideo-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **api.video** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apivideo-alternative": {
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
