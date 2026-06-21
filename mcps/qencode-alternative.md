# Qencode MCP Server

Automate video transcoding and live streaming via Qencode — manage tasks, start encodings, and orchestrate live streams directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/qencode-alternative)

## Overview
**Category:** developer-tools
**Tools Count:** 11

## Description
Connect your **Qencode** account to any AI agent to handle high-performance video processing and live broadcasting through natural conversation.

### What you can do

- **Video Transcoding** — Initialize tasks and start encoding processes with custom JSON queries for source and output formats
- **Live Streaming** — Create and manage live streams using RTMP, WebRTC, or SRT protocols with HLS/CMAF delivery
- **Simulcasting** — Add restreaming targets like YouTube or Twitch to your active live feeds automatically
- **Status Monitoring** — Track the real-time progress of multiple transcoding tasks (downloading, encoding, saving)
- **Infrastructure Management** — Manage custom CDN domains and update live stream configurations like DVR settings

### How it works

1. Subscribe to this server
2. Enter your Qencode API Key
3. Start processing video assets and managing broadcasts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Engineers** — automate complex transcoding workflows and monitor task queues without leaving the terminal or editor
- **Content Platforms** — orchestrate live streaming infrastructure and simulcasting targets programmatically
- **Product Teams** — integrate video processing status checks directly into project management or dev tools


## Available Tools
- **add_simulcast_target**: Add a simulcast target to a live stream
- **create_domain**: Create a custom CDN domain
- **create_live_stream**: Requires a live access token.

Create a new live stream
- **create_task**: Create a new transcoding task
- **get_access_token**: Required before creating tasks.

Get a session-based access token for transcoding
- **get_live_access_token**: Get an access token for live streaming
- **get_task_status**: Get the status of one or more transcoding tasks
- **start_encode**: Start a transcoding task with specific parameters
- **start_live_stream**: Start a live stream
- **stop_live_stream**: Stop a live stream
- **update_live_stream**: Update a live stream configuration


## Installation & Usage

To install and use the **Qencode** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qencode-alternative](https://vinkius.com/mcp/qencode-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
