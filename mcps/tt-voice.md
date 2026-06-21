# LiveKit Real-Time Rooms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tt-voice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication](../categories/communication.md)

Manage LiveKit voice and video rooms — create sessions, control participants, mute tracks, and broadcast data from any AI agent.

## Description
Connect your AI agents to **LiveKit**, the open-source framework and cloud platform for real-time voice, video, and AI agent communication. This MCP provides 10 tools to manage the full room lifecycle via the LiveKit Twirp Room Service API.

### What you can do

- **Room Management** — Create, list, and delete real-time voice/video rooms with configurable timeouts and participant limits
- **Participant Control** — List, inspect, update metadata, and remove participants from active rooms
- **Track Moderation** — Mute or unmute any published audio/video track for content moderation
- **Live Data Messaging** — Broadcast data payloads to all participants with reliable or lossy delivery modes
- **Room Metadata** — Dynamically update room-level metadata visible to all connected clients

### How it works

1. Subscribe to this server
2. Sign in to [**LiveKit Cloud**](https://cloud.livekit.io) (or configure your self-hosted LiveKit server)
3. Navigate to your project **Settings** to find your **API Key** and **API Secret**
4. Copy your server **Host URL** (e.g., `wss://your-project.livekit.cloud`)
5. Enter all three values into the credential fields below

### Who is this for?

- **AI Agent Developers** — programmatically manage voice rooms for conversational AI agents
- **Video Platform Builders** — automate room provisioning and participant lifecycle
- **Live Event Operators** — control moderation, muting, and data broadcasts in real-time sessions
- **Game Developers** — create dynamic voice channels tied to game state and matchmaking


## Available Tools (10)
- **create_room**: Participants can join it via access tokens.

Create a new LiveKit room with specified settings
- **list_rooms**: List all active rooms on the LiveKit server
- **delete_room**: Requires roomCreate permission.

Delete a room, disconnecting all participants
- **get_participant**: Get detailed information about a specific participant
- **list_participants**: List all participants currently in a room
- **mute_track**: Mute or unmute a participant's published track
- **remove_participant**: On LiveKit Cloud, their token is also revoked.

Remove a participant from a room
- **send_data**: Use "reliable" for guaranteed delivery or "lossy" for low-latency.

Send a data message to all participants in a room
- **update_participant_metadata**: Update a participant's metadata
- **update_room_metadata**: Use JSON strings for structured data.

Update the metadata of a room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LiveKit Real-Time Rooms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active rooms on my LiveKit server."

**🤖 AI Agent:**
> I've queried your LiveKit server. There are currently 3 active rooms: 'support-call-42' (2 participants), 'team-standup' (5 participants), and 'demo-room' (0 participants). Which one would you like to manage?

---

**👤 You:**
> "Create a room called 'interview-session' with a max of 3 participants."

**🤖 AI Agent:**
> Done! Room 'interview-session' has been created on your LiveKit server with a 10-minute empty timeout and a max of 3 participants. Participants can now join using an access token scoped to this room.

---

**👤 You:**
> "Remove the participant 'user-abc' from room 'support-call-42'."

**🤖 AI Agent:**
> Participant 'user-abc' has been removed from room 'support-call-42'. Their access token has been revoked and they will need a new token to rejoin.


## ❓ FAQ

**Q: Can I list all active rooms on my LiveKit server?**
Yes! Use the `list_rooms` tool. It calls the LiveKit RoomService ListRooms endpoint and returns all currently open rooms with their participant count, metadata, and creation time.

**Q: How do I mute a participant's microphone?**
First use `list_participants` to get the track SID for the participant's audio track. Then call `mute_track` with the room name, participant identity, track SID, and muted set to 'true'.

**Q: Does this work with self-hosted LiveKit servers?**
Yes! Just provide your self-hosted server's URL (e.g., https://livekit.yourserver.com) as the Host URL, along with the API Key and Secret from your server's config.yaml.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tt-voice](https://vinkius.com/mcp/tt-voice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LiveKit Real-Time Rooms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tt-voice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LiveKit Real-Time Rooms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tt-voice": {
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
