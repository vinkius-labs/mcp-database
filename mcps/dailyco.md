# Daily.co MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dailyco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage video calls and WebRTC infrastructure via Daily.co — create rooms, track participants, and control meeting sessions directly from your AI.

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


## Available Tools (50)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daily.co** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my current Daily rooms, limited to the last 10."

**🤖 AI Agent:**
> I've retrieved your rooms. You have 8 active rooms including 'onboarding-session', 'daily-standup', and 'support-chat-123'. Would you like the details for any specific one?

---

**👤 You:**
> "Create a new public room called 'community-hangout' with recording enabled."

**🤖 AI Agent:**
> The room 'community-hangout' has been created successfully. It is public and configured with recording properties. You can access it at: https://your-domain.daily.co/community-hangout

---

**👤 You:**
> "Who is currently in the 'emergency-room' and can you eject participant 'user-123'?"

**🤖 AI Agent:**
> There are currently 2 participants in 'emergency-room': 'admin-user' and 'user-123'. I am now proceeding to eject 'user-123' as requested.


## ❓ FAQ

**Q: Can I see exactly who is currently inside a video room?**
Yes. Use the `get_room_presence` tool with the room name. It returns a snapshot of all active participants currently connected to that specific session.

**Q: How do I create a private room that requires a token to join?**
You can use the `create_room` tool and set the `privacy` parameter to 'private'. You can also pass additional configuration in the `properties` JSON field.

**Q: Is it possible to remove a disruptive participant from a call?**
Yes. The `eject_participants` tool allows you to kick specific users by their IDs. You can also set the `ban` flag to true to prevent them from re-entering the room.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dailyco](https://vinkius.com/mcp/dailyco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Daily.co** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dailyco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Daily.co** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dailyco": {
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
