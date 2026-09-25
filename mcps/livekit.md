# LiveKit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/livekit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage real-time video, audio, and data sessions via LiveKit — create rooms, manage participants, and trigger recordings directly from your AI agent.

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


## Available Tools (41)
- **create_dispatch**: Specify the agent name and room name.

Explicitly trigger a named agent to join a specific room
- **create_ingress**: Specify the input type and name.

Provision an ingress point (RTMP, WHIP, or URL pull)
- **create_room**: Create a room with specific settings
- **create_sip_dispatch_rule**: Specify the rule name and required configurations.

Map incoming calls to specific rooms based on phone numbers or pins
- **create_sip_inbound_trunk**: Provide a unique name for the trunk.

Define how incoming SIP calls are handled
- **create_sip_outbound_trunk**: Provide a unique name for the trunk.

Define a trunk for dialing out
- **create_sip_participant**: Provide all necessary identifiers.

Dial a SIP number and bring them into a LiveKit room
- **delete_dispatch**: Provide both the dispatch ID and the room name.

Remove a dispatch rule
- **delete_ingress**: Provide the ingress ID to delete the resource.

Remove an ingress point
- **delete_room**: Specify the room name as the only required argument.

Forcibly disconnect all participants and delete the room
- **delete_sip_dispatch_rule**: Provide the specific SIP Dispatch Rule ID to delete the resource.

Remove a SIP dispatch rule
- **delete_sip_trunk**: Use the specific SIP Trunk ID for deletion.

Remove a SIP trunk configuration
- **get_participant**: Supply both the room name and the participant’s identity.

Get info for a specific participant
- **list_dispatch**: Provide the room name to retrieve the list.

List dispatches for a room
- **list_egress**: Filter results using room name or egress ID.

List active egress jobs
- **list_ingress**: Filter results using room name or ingress ID.

List provisioned ingresses
- **list_participants**: Provide the room name to execute the query.

List participants in a room
- **list_phone_numbers**: List numbers owned by the project
- **list_rooms**: List active/open rooms
- **list_sip_inbound_trunk**: List configured SIP inbound trunks
- **list_sip_outbound_trunk**: List configured SIP outbound trunks
- **mute_published_track**: Provide the room name, participant identity, and track SID.

Mute/unmute a participant's track
- **purchase_phone_number**: Specify the phone number to be purchased.

Buy a number and optionally assign a SIP dispatch rule
- **release_phone_numbers**: Provide the phone number you wish to release.

Release a number back to the inventory
- **remove_participant**: Supply both the room name and the participant’s identity.

Kick a participant from a room
- **search_phone_numbers**: Provide both codes for accurate results.

Search for available numbers by country/area code
- **send_data**: Specify the room name and the data payload.

Send data packets to participants
- **start_participant_egress**: Provide the room name and participant identity.

Record a specific participant's audio and video
- **start_room_composite_egress**: Provide the room name and the desired layout name.

Record an entire room using a web layout
- **start_track_composite_egress**: Provide both audio and video track IDs.

Record one audio and one video track together
- **start_track_egress**: Provide the room name and the specific track ID.

Export a single track without transcoding
- **start_web_egress**: Provide the URL to be recorded.

Record any web page
- **stop_egress**: Provide the egress ID to terminate the job.

Stop an active egress
- **transfer_sip_participant**: Ensure the participant and room names are correct.

Transfer an active SIP call to another number or URI
- **update_ingress**: Use the ingress ID to identify the resource.

Update room or participant settings for a reusable ingress
- **update_layout**: Use the egress ID to target the correct job.

Change the web layout of an active RoomComposite egress
- **update_participant**: Specify the room name and participant identity.

Update metadata or permissions for a participant
- **update_phone_number**: Provide the number and the new rule ID.

Change the dispatch rule for a number
- **update_room_metadata**: Provide the room name and the new metadata string.

Update room-wide metadata
- **update_stream**: Use the egress ID to identify the stream.

Add/remove RTMP/SRT output URLs from an active stream
- **update_subscriptions**: Provide the room name and participant identity.

Subscribe/unsubscribe a participant from specific tracks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LiveKit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently active rooms in my LiveKit instance."

**🤖 AI Agent:**
> I've retrieved the active rooms. You have 3 rooms running: 'Main-Lobby' (2 participants), 'Gaming-Zone' (5 participants), and 'Support-Desk' (0 participants).

---

**👤 You:**
> "Create a new room called 'Strategy-Meeting' with a max of 10 participants."

**🤖 AI Agent:**
> The room 'Strategy-Meeting' has been successfully created with a limit of 10 participants and a default empty timeout.

---

**👤 You:**
> "Mute the audio track for participant 'user_99' in the 'Main-Lobby' room."

**🤖 AI Agent:**
> I've sent the command to mute the track 'TR_XXXXXXXX' for 'user_99' in 'Main-Lobby'. The participant is now muted.


## ❓ FAQ

**Q: Can I remotely mute a participant who has background noise?**
Yes. Use the `mute_published_track` tool by providing the room name, participant identity, and the specific track SID. You can set the `muted` boolean to true to silence them immediately.

**Q: Is it possible to record a session for later viewing?**
Absolutely. You can use `start_room_composite_egress` to record an entire room using a web layout, or `start_web_egress` to record a specific URL. These tools leverage LiveKit's Egress service.

**Q: How do I kick a disruptive user from a room?**
You can use the `remove_participant` tool. Simply provide the room name and the identity of the participant you wish to disconnect.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/livekit](https://vinkius.com/en/ai-agent-connect/livekit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LiveKit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `livekit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LiveKit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "livekit": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
