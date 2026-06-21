# Cloudflare Stream MCP Server

Manage video infrastructure via Cloudflare Stream—list videos, manage live inputs, and handle uploads directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudflare-stream)

## Overview
**Category:** industry-titans
**Tools Count:** 26

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


## Installation & Usage

To install and use the **Cloudflare Stream** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudflare-stream](https://vinkius.com/mcp/cloudflare-stream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
