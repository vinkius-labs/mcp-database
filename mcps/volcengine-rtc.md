# Volcengine RTC MCP Server

Bring ByteDance's internal RTC Engine to your AI workflow. Administrate audio/video calls, manage servers, and start Mixes.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/volcengine-rtc)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Empower your Agent with **Volcengine RTC**, the exact same Real-Time Communication backbone powering ByteDance's most prominent applications like TikTok and Douyin globally. This plugin provides 10 core administrative functions to manipulate streams autonomously.

### What you can do

- **Real-time Live Stream Operation** — Mute and unmute broadcaster audio/video feeds directly through natural language
- **Automated Expulsions** — Remove abusive streamers via Room ID controls dynamically
- **MCU Mixing & Recording** — Spin up cloud mixing or save streams directly to VOD storage effortlessly
- **Topology Oversight** — Query active servers, discover users inside those rooms and evaluate network drop rates

### How it works

1. Install this MCP server
2. Log into the Volcengine IAM Console to get an **Access Key (AK)** and **Secret Key (SK)**
3. Plug those alongside your **RTC App ID** into your client. The Vurb extension engine will dynamically convert the AI's natural language into signed HMAC-SHA256 REST API commands.

### Who is this for?

- **Stream Operators** — Command AI to instantly mute streamers acting inappropriately without fumbling through dashboards
- **Network Analysts** — Analyze dropped frame rates to determine poor connectivity in a specific node purely from prompt traces


## Available Tools
- **get_active_rooms**: List all active RTC rooms in Volcengine
- **get_quality_metrics**: Get deep dive metrics of an RTC room
- **get_room_users**: Get list of users in a Volcengine room
- **kick_user**: Kick a user from a Volcengine RTC room
- **mute_stream**: StreamType should be "audio" or "video".

Mute a specific stream output (audio or video)
- **start_cloud_record**: Start Volcengine Cloud Recording
- **start_transcode**: Start Cloud MCU stream transcoding
- **stop_cloud_record**: Stop Volcengine Cloud Recording
- **stop_transcode**: Stop MCU stream transcoding
- **unmute_stream**: StreamType should be "audio" or "video".

Unmute a previously muted stream output


## Installation & Usage

To install and use the **Volcengine RTC** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/volcengine-rtc](https://vinkius.com/mcp/volcengine-rtc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
