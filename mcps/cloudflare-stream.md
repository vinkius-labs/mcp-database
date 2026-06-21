# Cloudflare Stream MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudflare-stream)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage video infrastructure via Cloudflare Stream—list videos, manage live inputs, and handle uploads directly from any AI agent.

## Description
Connect your **Cloudflare Stream** account to any AI agent to manage your video delivery and live streaming workflows through natural conversation.

### What you can do

- **Video Management** — List all videos in your account, fetch specific metadata, and filter by status (ready, in-progress, error) or type (vod, live).
- **Live Streaming** — Create and manage live inputs, configure recording options, and list simulcast outputs for platforms like YouTube or Twitch.
- **Content Editing** — Update video metadata, set allowed origins for security, and schedule automatic deletions.
- **Upload Workflows** — Initiate video uploads using the TUS protocol with custom metadata and size specifications.
- **Deletion Control** — Permanently remove videos or live inputs when they are no longer needed.

### How it works

1. Subscribe to this server
2. Enter your Cloudflare Account ID and API Token
3. Start managing your video library and live streams from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Media Teams** — quickly check video statuses and manage metadata without leaving the chat interface.
- **Developers** — integrate video upload and management logic into coding workflows or automated agents.
- **Live Streamers** — monitor live inputs and configure simulcast destinations on the fly.


## Available Tools
- **copy_audio_track**: Add an audio track via URL
- **create_live_input**: Can specify metadata and recording options.

Creates a live input for streaming video to Cloudflare
- **create_live_output**: Create a simulcast output for a live input
- **create_m4a_download**: Enable M4A audio downloads for a video
- **create_mp4_download**: Enable MP4 downloads for a video
- **create_signing_key**: Create a Stream Signing Key
- **create_watermark**: Create a watermark profile
- **delete_live_input**: Delete a live input
- **delete_live_output**: Delete a simulcast output
- **delete_video**: Deletes a video and its copies
- **edit_video**: Update metadata or settings for a video
- **generate_caption**: Generate AI captions for a video
- **get_storage_usage**: Retrieve account-wide storage statistics
- **get_video**: Retrieve details for a single video
- **get_webhook**: View webhook configuration
- **initiate_upload**: Requires upload length in bytes and base64 encoded metadata.

Initiates a video upload using the TUS protocol
- **list_audio_tracks**: List additional audio tracks for a video
- **list_captions**: List text tracks (subtitles/captions) for a video
- **list_downloads**: List available downloads for a video
- **list_live_inputs**: List live inputs
- **list_live_outputs**: g., YouTube, Twitch) for a specific live input.

List simulcast outputs for a live input
- **list_signing_keys**: List Stream Signing Keys
- **list_videos**: Can filter by status, type, or search term.

List videos in your Cloudflare Stream account
- **list_watermarks**: List watermark profiles
- **update_webhook**: Create or update webhook configuration
- **upload_caption**: Upload a VTT caption file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudflare Stream** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 videos in my Cloudflare Stream account."

**🤖 AI Agent:**
> I've retrieved your latest videos. You have 10 videos listed, including 'Product Demo' (Ready) and 'Keynote 2023' (Ready). Would you like details on a specific one?

---

**👤 You:**
> "Create a new live input named 'Weekly Webinar' with automatic recording enabled."

**🤖 AI Agent:**
> Live input 'Weekly Webinar' has been created successfully. Your RTMPS URL and Stream Key are ready. Recording is set to 'automatic'.

---

**👤 You:**
> "Show me the details for video ID 4f92b3c8e1a04d56b7f8c9d0e1f2a3b4."

**🤖 AI Agent:**
> Fetching details... Video 'Marketing Launch' is 120MB, status is 'ready', and it was uploaded on Oct 12th. It currently requires signed URLs for viewing.


## ❓ FAQ

**Q: Can I filter my video list to see only videos that are ready to watch?**
Yes! Use the `list_videos` tool and set the `status` parameter to 'ready'. You can also filter by type (vod or live) and search for specific names.

**Q: How do I create a new live streaming endpoint?**
You can use the `create_live_input` tool. You can optionally provide metadata like a stream name and configure whether the stream should be automatically recorded.

**Q: Is it possible to update the metadata of an existing video?**
Absolutely. Use the `edit_video` tool with the video's identifier. You can update the `meta` object, change `allowedOrigins`, or toggle `requireSignedURLs`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudflare-stream](https://vinkius.com/mcp/cloudflare-stream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloudflare Stream** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cloudflare-stream` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloudflare Stream** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudflare-stream": {
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
