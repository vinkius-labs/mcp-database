# LiveKit MCP Server

Manage real-time video, audio, and data sessions via LiveKit — create rooms, manage participants, and trigger recordings directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/livekit)

## Overview
**Category:** communication-messaging
**Tools Count:** 41

## Description
Connect your **LiveKit** infrastructure to any AI agent to orchestrate real-time communication environments through natural language. This server provides comprehensive control over WebRTC sessions, participant permissions, and media recording.

### What you can do

- **Room Lifecycle** — Create, list, and delete rooms with custom timeouts, participant limits, and metadata.
- **Participant Control** — List active participants, retrieve detailed info, or remove users from a session.
- **Media Management** — Remotely mute or unmute specific tracks (audio/video) for any participant.
- **Real-time Data** — Send data packets (Base64 encoded) to specific participants or entire rooms for custom signaling.
- **Recording & Egress** — Start room-wide recordings using web layouts or record specific web pages via the Egress API.
- **Metadata & Permissions** — Update room-wide metadata or modify individual participant permissions and subscriptions on the fly.

### How it works

1. Subscribe to this server
2. Enter your LiveKit Server URL and API Token/Secret
3. Start managing your real-time infrastructure from Claude, Cursor, or any MCP-compatible client

No more manual dashboard navigation to check who is in a room or to force-mute a noisy participant. Your AI acts as a real-time session administrator.


## Available Tools
- **create_dispatch**: Explicitly trigger a named agent to join a specific room
- **create_ingress**: Provision an ingress point (RTMP, WHIP, or URL pull)
- **create_room**: Create a room with specific settings
- **create_sip_dispatch_rule**: Map incoming calls to specific rooms based on phone numbers or pins
- **create_sip_inbound_trunk**: Define how incoming SIP calls are handled
- **create_sip_outbound_trunk**: Define a trunk for dialing out
- **create_sip_participant**: Dial a SIP number and bring them into a LiveKit room
- **delete_dispatch**: Remove a dispatch rule
- **delete_ingress**: Remove an ingress point
- **delete_room**: Forcibly disconnect all participants and delete the room
- **delete_sip_dispatch_rule**: Remove a SIP dispatch rule
- **delete_sip_trunk**: Remove a SIP trunk configuration
- **get_participant**: Get info for a specific participant
- **list_dispatch**: List dispatches for a room
- **list_egress**: List active egress jobs
- **list_ingress**: List provisioned ingresses
- **list_participants**: List participants in a room
- **list_phone_numbers**: List numbers owned by the project
- **list_rooms**: List active/open rooms
- **list_sip_inbound_trunk**: List configured SIP inbound trunks
- **list_sip_outbound_trunk**: List configured SIP outbound trunks
- **mute_published_track**: Mute/unmute a participant's track
- **purchase_phone_number**: Buy a number and optionally assign a SIP dispatch rule
- **release_phone_numbers**: Release a number back to the inventory
- **remove_participant**: Kick a participant from a room
- **search_phone_numbers**: Search for available numbers by country/area code
- **send_data**: Send data packets to participants
- **start_participant_egress**: Record a specific participant's audio and video
- **start_room_composite_egress**: Record an entire room using a web layout
- **start_track_composite_egress**: Record one audio and one video track together
- **start_track_egress**: Export a single track without transcoding
- **start_web_egress**: Record any web page
- **stop_egress**: Stop an active egress
- **transfer_sip_participant**: Transfer an active SIP call to another number or URI
- **update_ingress**: Update room or participant settings for a reusable ingress
- **update_layout**: Change the web layout of an active RoomComposite egress
- **update_participant**: Update metadata or permissions for a participant
- **update_phone_number**: Change the dispatch rule for a number
- **update_room_metadata**: Update room-wide metadata
- **update_stream**: Add/remove RTMP/SRT output URLs from an active stream
- **update_subscriptions**: Subscribe/unsubscribe a participant from specific tracks


## Installation & Usage

To install and use the **LiveKit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/livekit](https://vinkius.com/mcp/livekit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
