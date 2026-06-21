# api.video MCP Server

Automate video workflows via api.video — upload, stream, and analyze video content directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/apivideo-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 49

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


## Available Tools
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


## Installation & Usage

To install and use the **api.video** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apivideo-alternative](https://vinkius.com/mcp/apivideo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
