# Daily.co MCP Server

Manage video calls and WebRTC infrastructure via Daily.co — create rooms, track participants, and control meeting sessions directly from your AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dailyco)

## Overview
**Category:** communication-messaging
**Tools Count:** 50

## Description
Connect your **Daily.co** account to any AI agent to orchestrate real-time video and audio communication workflows through natural language.

### What you can do

- **Room Management** — Create, list, update, and delete video rooms. Configure privacy settings (public/private) and custom properties on the fly.
- **Participant Control** — Monitor real-time presence to see who is in a call and eject participants or ban them when necessary.
- **Domain Configuration** — Retrieve and set top-level domain settings for your Daily infrastructure.
- **Session Data** — Sync and retrieve custom session data across all participants to maintain state during meetings.
- **App Messaging** — Send data payloads to participants within a room to trigger client-side actions or notifications.

### How it works

1. Subscribe to this server
2. Enter your Daily API Key
3. Start managing your video infrastructure from Claude, Cursor, or any MCP-compatible client

Your AI acts as a virtual operator, capable of spinning up meeting rooms for support tickets or auditing active sessions without you ever touching a dashboard.

### Who is this for?

- **Developers** — quickly test room configurations and manage WebRTC infrastructure directly from the code editor.
- **Support & Ops Teams** — monitor active meeting presence and manage participant access for webinars or private consultations.
- **Product Managers** — automate the creation of unique meeting links for specific project workflows or client calls.


## Available Tools
- **buy_phone_number**: Purchase a specific or random number
- **create_batch_job**: Submit a batch processor job
- **create_meeting_token**: Create a meeting token
- **create_room**: Create a new room
- **create_webhook**: Create a webhook
- **delete_batch_job**: Delete a batch job
- **delete_recording**: Delete a recording reference
- **delete_room**: Delete a room
- **delete_webhook**: Delete a webhook
- **eject_participants**: Kick participants from a room
- **get_batch_job_access_link**: Get download links for finished jobs
- **get_batch_job**: Get batch job status
- **get_domain**: Retrieve domain configuration
- **get_global_presence**: List all active participants on the domain
- **get_logs**: Retrieve detailed call logs and metrics
- **get_meeting_participants**: List participants in a session
- **get_meeting**: Get details for a specific session
- **get_recording_access_link**: Generate a time-limited S3 download link
- **get_recording**: Get recording information
- **get_room_presence**: Get active participants in a room
- **get_room**: Retrieve a specific room
- **get_session_data**: Retrieve meeting session data
- **get_webhook**: Get specific webhook info
- **list_available_numbers**: Search for numbers by areacode or region
- **list_batch_jobs**: List all batch jobs
- **list_meetings**: List meeting sessions
- **list_purchased_numbers**: List numbers owned by your domain
- **list_recordings**: Supports pagination.

List cloud recordings
- **list_rooms**: Supports pagination.

List rooms
- **list_webhooks**: List webhooks
- **release_phone_number**: Release a number
- **send_app_message**: Send data to participants
- **send_dtmf**: Send DTMF tones to a session
- **set_domain**: Set domain configuration
- **set_session_data**: Sync data to all participants
- **start_dial_out**: Call a sipUri or phoneNumber
- **start_live_streaming**: Start RTMP/HLS streaming
- **start_recording**: Start a recording
- **start_transcription**: Start real-time transcription
- **stop_dial_out**: End a dial-out session
- **stop_live_streaming**: Stop streaming
- **stop_recording**: Stop an active recording
- **stop_transcription**: Stop transcription
- **update_live_streaming**: Update layout or endpoints for streaming
- **update_permissions**: Update participant permissions
- **update_recording**: Update layout of an active recording
- **update_room**: Modify room privacy or configuration
- **update_transcription**: Update participants being transcribed
- **update_webhook**: Update or re-activate a failed webhook
- **validate_meeting_token**: Validate a meeting token


## Installation & Usage

To install and use the **Daily.co** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailyco](https://vinkius.com/mcp/dailyco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
