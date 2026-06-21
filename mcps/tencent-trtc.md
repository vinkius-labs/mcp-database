# Tencent TRTC MCP Server

Bring Tencent's Dominant Real-Time Communications Engine to your AI workflow. Manage rooms, cloud recordings, and call metrics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-trtc)

## Overview
**Category:** industry-titans
**Tools Count:** 11

## Description
Equip your AI agent with **Tencent TRTC** (Tencent Real-Time Communication), the underlying video-conferencing technology empowering massive platforms globally. This MCP server offers 10 deep tools to administrate live-streaming rooms automatically.

### What you can do

- **Session & User Administration** — Kick malicious users from calls, dismiss full rooms, and track active users in real-time
- **Cloud Processing** — Autonomously start MCU stream mixing or coordinate high-definition cloud recordings to Tencent VOD
- **Quality Assessment** — Parse and assess real-time call performance matrices and dropped-frame analytics directly

### How it works

1. Subscribe to this server
2. Insert your **Tencent SecretId**, **SecretKey**, and **SdkAppId** from your [Developer Console](https://console.cloud.tencent.com/api/manage)
3. Inject the server into your LLM logic to use it as an automated stream backend

### Who is this for?

- **Live-stream Moderators** — Empower LLMs to automatically kick rogue broadcasters
- **Cloud DevOps** — Easily analyze network quality to diagnose why a client video is lagging
- **Infrastructure Managers** — Manage massive cloud recordings remotely


## Available Tools
- **describe_call_detail_info**: Get granular call quality metrics
- **describe_room_info**: Get TRTC room session details
- **describe_trtc_usage**: Get aggregated TRTC usage statistics
- **describe_user_info**: Requires CommId format: SdkAppId_CreateTime.

Query user list for a specific call session
- **dismiss_room**: Terminate a TRTC room session
- **remove_user**: Remove users from a TRTC room
- **remove_user_by_str_room_id**: Remove users from a TRTC room by string room ID
- **start_cloud_recording**: Start cloud recording for a TRTC room
- **start_mcu_mix**: Start MCU mix transcoding for a room
- **stop_cloud_recording**: Stop an active cloud recording task
- **stop_mcu_mix**: Stop MCU mix transcoding for a room


## Installation & Usage

To install and use the **Tencent TRTC** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-trtc](https://vinkius.com/mcp/tencent-trtc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
