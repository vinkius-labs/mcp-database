# ZegoCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zegocloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage real-time communication (RTC) and interactive messaging — kick users, stop streams, and send peer messages via AI.

## Description
Connect your **ZegoCloud** infrastructure to any AI agent to moderate and control your real-time video, voice, and messaging environments through natural language.

### What you can do

- **User Moderation** — Instantly remove disruptive users from specific virtual rooms using the kickout tool.
- **Stream Control** — Manage active live streams by stopping specific stream IDs to maintain content quality and security.
- **Direct Messaging** — Send peer-to-peer text messages or system commands (ZIM) between users for real-time interaction.
- **Room Management** — Orchestrate your communication rooms without manually accessing the admin dashboard.

### How it works

1. Subscribe to this server
2. Enter your ZegoCloud App ID, Server Secret, and API URL
3. Start moderating calls and managing messages from Claude, Cursor, or any MCP client

### Who is this for?

- **Community Moderators** — quickly remove users or stop unauthorized streams during live events.
- **Support Engineers** — send technical commands or messages to users directly from the console.
- **Developers** — test and manage RTC workflows and messaging logic without leaving the code editor.


## Available Tools
- **kickout_user**: Kick a user out of a room
- **send_peer_message**: Send a peer-to-peer message
- **stop_publish**: Stop publishing a stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ZegoCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Kick user 'user_88' from room 'main_lobby' for inappropriate behavior."

**🤖 AI Agent:**
> I have successfully removed 'user_88' from the room 'main_lobby'. The reason provided was 'inappropriate behavior'.

---

**👤 You:**
> "Stop the broadcast for stream ID 'stream_v_123'."

**🤖 AI Agent:**
> The stream 'stream_v_123' has been stopped. The publishing session is now terminated.

---

**👤 You:**
> "Send a text message 'Hello from support' to user 'client_01' from 'admin_user'."

**🤖 AI Agent:**
> Message sent successfully. 'client_01' has received the text: 'Hello from support'.


## ❓ FAQ

**Q: Can I remove a specific user from a video room if they are violating terms?**
Yes. Use the `kickout_user` tool by providing the Room ID and User ID. You can also include a custom reason for the removal.

**Q: How do I stop a live stream that is currently broadcasting?**
Simply use the `stop_publish` tool with the specific Stream ID. This will immediately terminate the broadcast for that stream.

**Q: Is it possible to send a private system command to a user's application?**
Yes. The `send_peer_message` tool allows you to send messages with type '2' (Command), which can be used to trigger logic within the recipient's app.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zegocloud](https://vinkius.com/mcp/zegocloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ZegoCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zegocloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ZegoCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zegocloud": {
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
