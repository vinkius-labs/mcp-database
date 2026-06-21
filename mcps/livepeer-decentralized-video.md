# Livepeer (Decentralized Video) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/livepeer-decentralized-video)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/livepeer-decentralized-video-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/livepeer-decentralized-video-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage decentralized video infrastructure via Livepeer — upload assets, manage live streams, create clips, and monitor viewership metrics directly from any AI agent.

## Description
Connect your **Livepeer** account to any AI agent to orchestrate decentralized video workflows through natural conversation.

### What you can do

- **Asset Management** — Upload videos via external URLs (HTTP, IPFS, Arweave) using `upload_asset_via_url` or request direct upload endpoints.
- **Live Streaming** — Create, update, and terminate live streams with `create_stream` and `terminate_stream`.
- **On-Demand Clips** — Generate short video clips from active live streams using `create_clip` with precise timestamps.
- **Analytics & Metrics** — Access detailed usage statistics and real-time audience metrics with `get_usage_metrics` and `get_realtime_viewership`.
- **Multistreaming** — Configure multistream targets to broadcast your content across multiple platforms simultaneously.

### How it works

1. Subscribe to this server
2. Enter your Livepeer API Key
3. Start managing your video infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Engineers** — automate the deployment and monitoring of streaming pipelines without manual dashboard navigation.
- **Content Creators** — quickly generate clips and check stream health straight from their workspace.
- **DApp Developers** — integrate decentralized video features into applications using natural language commands.


## Available Tools
- **create_clip**: Create a short video clip from a live stream
- **create_multistream_target**: Create a multistream target (e.g., Twitch, YouTube)
- **create_room**: Create a real-time WebRTC multi-participant video room
- **create_room_user**: Create a user for a specific room
- **create_stream**: Create a new live stream
- **create_transcode_job**: Create an on-demand video transcode job
- **create_webhook**: Create a webhook to subscribe to real-time events
- **delete_asset**: Delete an asset
- **delete_multistream_target**: Delete a multistream target
- **delete_stream**: Delete a stream
- **delete_webhook**: Delete a webhook
- **get_asset**: Retrieve details of a specific asset
- **get_multistream_target**: Retrieve a multistream target
- **get_playback_info**: Retrieve metadata and URLs for playing back assets or streams
- **get_realtime_viewership**: Query real-time viewership metrics
- **get_session_clips**: Retrieve clips associated with a specific session
- **get_session**: Retrieve details of a specific broadcast session
- **get_stream**: Retrieve details of a specific stream
- **get_task**: Retrieve a specific task (e.g., upload, transcode)
- **get_usage_metrics**: Query usage metrics (total minutes transcoded and delivered)
- **get_viewership_metrics**: Query viewership metrics (breakdown by device, browser, location)
- **get_webhook**: Retrieve a specific webhook
- **list_assets**: Retrieve all assets
- **list_sessions**: Retrieve all broadcast sessions
- **list_streams**: Retrieve all streams
- **list_tasks**: Retrieve all tasks
- **request_asset_upload**: Request a direct upload URL for a new asset
- **start_room_egress**: Broadcast a room session to a Livepeer Stream (RTMP Egress)
- **terminate_stream**: Terminate an active stream
- **update_asset**: Update an existing asset
- **update_multistream_target**: Update a multistream target
- **update_stream**: Update an existing stream
- **update_webhook**: Update a webhook
- **upload_asset_via_url**: Upload an asset using an external URL (HTTP, IPFS, Arweave)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Livepeer (Decentralized Video)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my video assets on Livepeer."

**🤖 AI Agent:**
> I've retrieved your assets. You have 3 videos: 'Intro.mp4' (ID: asset_123), 'Tutorial.mov' (ID: asset_456), and 'Webinar_Rec.mp4' (ID: asset_789). Would you like details on any of them?

---

**👤 You:**
> "Create a new live stream called 'Community Call'."

**🤖 AI Agent:**
> Stream 'Community Call' has been created successfully. Your Stream Key is `xxxx-xxxx-xxxx` and the RTMP ingest URL is `rtmp://rtmp.livepeer.com/live`. Ready to broadcast!

---

**👤 You:**
> "Show me the usage metrics for my account."

**🤖 AI Agent:**
> Fetching usage data... This month you have transcoded 450 minutes of video and delivered 1.2TB of data via the CDN. Your current storage usage is at 85GB.


## Installation & Usage

To install and use the **Livepeer (Decentralized Video)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/livepeer-decentralized-video](https://vinkius.com/mcp/livepeer-decentralized-video)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
