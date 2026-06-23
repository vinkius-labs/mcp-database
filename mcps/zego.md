# ZEGO / 即构科技 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zego)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Leading global RTC and IM platform — manage rooms, users, and media streams via AI.

## Description
Empower your AI agent to orchestrate your real-time communication infrastructure with **ZEGO** (即构科技), the premier provider of global video and audio RTC services. By connecting ZEGO to your agent, you transform complex room management, stream control, and user status tracking into a natural conversation. Your agent can instantly retrieve active room lists, monitor user counts, force-stop media streams, and audit service usage statistics without you ever needing to navigate multiple technical dashboards. Whether you are building an automated moderation system for live rooms or monitoring cross-regional connectivity, your agent acts as a real-time RTC operations assistant, providing accurate and reliable results from a single, authorized source.

### What you can do

- **Room Orchestration** — List active rooms, retrieve detailed metadata, and monitor real-time user activity.
- **User Management** — Track user status (online/offline), list members in specific rooms, and manage access (kick users).
- **Stream Control** — Monitor active media streams and force-terminate unauthorized or problematic broadcasts.
- **Usage Auditing** — Retrieve comprehensive audio and video duration statistics for specific time ranges.
- **Operational Insights** — Monitor total online user counts and API connectivity status to ensure system-wide health.

### How it works

1. Subscribe to this server
2. Enter your ZEGO AppID and ServerSecret
3. Start managing your RTC infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Moderators** — manage live rooms and enforce safety policies through natural language queries.
- **Operations Teams** — monitor real-time usage and audit system connectivity directly from your AI-powered workspace.
- **Developers** — integrate professional RTC and IM APIs into your AI-driven daily routines.
- **ZEGO Power Users** — integrate your existing communication workflows into your AI-driven daily routines.


## Available Tools (8)
- **check_user_status**: Check status of multiple users
- **get_online_count**: Get total online user count
- **get_room_streams**: List active streams in a room
- **get_room_users**: List users in a room
- **get_usage_stats**: Get service usage statistics
- **kick_room_user**: Kick user from room
- **list_rooms**: List active rooms
- **stop_media_stream**: Force stop a stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZEGO / 即构科技** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active rooms in our ZEGO project."

**🤖 AI Agent:**
> I've retrieved the list of active rooms. You currently have 3 rooms online: 'Room_A' (12 users), 'Room_B' (5 users), and 'Room_C' (45 users). Would you like to see the members list for one of these rooms?

---

**👤 You:**
> "Check the status for these users: 'user_01,user_02'."

**🤖 AI Agent:**
> I've checked the status for the requested users. 'user_01' is currently 'Online' and participating in 'Room_A'. 'user_02' is currently 'Offline'. Should I check the total online count for the whole project?

---

**👤 You:**
> "What is our video usage duration for the last 7 days?"

**🤖 AI Agent:**
> I've retrieved the usage statistics. Over the last 7 days, your project has consumed a total of 15,240 minutes of video and 8,500 minutes of audio. Would you like a daily breakdown of this usage?


## ❓ FAQ

**Q: How do I find my ZEGO AppID and ServerSecret?**
Log in to the [ZEGO Admin Console](https://console.zego.im/), create or select a project, and you will find your AppID and ServerSecret in the project configuration or basic information section.

**Q: What is the SignatureNonce used for?**
The SignatureNonce is a random string used to prevent replay attacks. This server automatically generates a fresh nonce for every request to ensure high security for your RTC management.

**Q: Can I kick a user from a specific room?**
Yes! Use the `kick_room_user` tool with the target RoomId and UserId. You can also provide a custom message that the user will see when they are disconnected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zego](https://vinkius.com/mcp/zego)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZEGO / 即构科技** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zego` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZEGO / 即构科技** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zego": {
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
