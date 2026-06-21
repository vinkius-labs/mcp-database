# Limelight Networks (Edgio CDN & Streaming API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/limelight-networks-edgio-cdn-streaming-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/limelight-networks-edgio-cdn-streaming-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/limelight-networks-edgio-cdn-streaming-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage Edgio (formerly Limelight/Uplynk) streaming services — control VOD assets, linear channels, and live events directly through AI.

## Description
Integrate **Edgio (formerly Limelight Networks and Uplynk)** into your AI workflows to orchestrate high-scale video delivery and streaming operations.

### What you can do

- **VOD Asset Management** — List, inspect, update, and delete Video-on-Demand assets within your CMS library.
- **Linear Channels** — Monitor and configure linear channel settings and schedules for continuous broadcasting.
- **Live Event Control** — Create, start, and stop live events with precise signaling for real-time streaming workflows.
- **Playback & Preplay** — Initialize secure playback sessions with SSAI (Server-Side Ad Insertion) and retrieve HLS/DASH manifests.
- **Operational Logs** — Access system logs and playback reports to monitor delivery performance and troubleshoot issues.

### How it works

1. Subscribe to this server
2. Provide your Edgio (Uplynk) Owner ID and API Key
3. Start managing your streaming infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Streaming Engineers** — Automate the lifecycle of live events and VOD assets without manual dashboard navigation.
- **Content Managers** — Update metadata and organize channel schedules through natural language commands.
- **DevOps Teams** — Integrate CDN and streaming controls into CI/CD pipelines or monitoring agents.


## Available Tools
- **create_event**: Creates a new live event
- **delete_asset**: Permanently removes an asset from the system
- **get_asset**: Retrieves detailed metadata for a specific asset
- **get_channel**: Retrieves configuration and status for a channel
- **get_dash_manifest**: Get DASH manifest for video playback
- **get_hls_manifest**: Get HLS manifest for video playback
- **get_playback_report**: Retrieves playback statistics (views, duration, etc.)
- **initialize_preplay_session**: Initialize a playback session for SSAI and security
- **list_assets**: Returns a list of all assets in your account
- **list_channels**: Lists all configured linear channels
- **list_events**: Lists all scheduled and active live events
- **list_logs**: Lists available log files for download
- **start_event**: Signals the start of a live event
- **stop_event**: Signals the end of a live event
- **update_asset**: Updates metadata (title, tags, etc.) for an asset
- **update_channel**: Updates channel settings or schedule
- **upload_slice**: Upload video segments for encoding and storage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Limelight Networks (Edgio CDN & Streaming API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all VOD assets currently in my Edgio account."

**🤖 AI Agent:**
> I've retrieved your VOD library. You have 12 assets, including 'Product_Launch_2024' (ID: a1b2c3) and 'Tutorial_Series_01' (ID: d4e5f6). Would you like details on a specific one?

---

**👤 You:**
> "Start the live event with ID 'live_event_998'."

**🤖 AI Agent:**
> The signal to start live event 'live_event_998' has been sent successfully. The stream is now transitioning to active status.

---

**👤 You:**
> "Initialize a playback session for asset 'd4e5f6' with ad configuration 'midroll_test'."

**🤖 AI Agent:**
> Playback session initialized. Here is your HLS URL: https://content.uplynk.com/d4e5f6.m3u8?pbs=xyz123&ad=midroll_test. The session is ready for secure delivery.


## Installation & Usage

To install and use the **Limelight Networks (Edgio CDN & Streaming API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/limelight-networks-edgio-cdn-streaming-api](https://vinkius.com/mcp/limelight-networks-edgio-cdn-streaming-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
