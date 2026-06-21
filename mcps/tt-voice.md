# LiveKit Real-Time Rooms MCP Server

Manage LiveKit voice and video rooms — create sessions, control participants, mute tracks, and broadcast data from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tt-voice)

## Overview
**Category:** communication
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **LiveKit Real-Time Rooms** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tt-voice](https://vinkius.com/mcp/tt-voice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
