# Netease Yunxin IM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netease-yunxin-im)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI Agent with Netease Yunxin to massively manage Live Chat Rooms, moderate IM participants, and broadcast messages.

## Description
Connect your LLMs directly to **Netease Yunxin** (网易云信), the prominent IM API platform supporting massive concurrency arrays in Asia. This MCP encapsulates 11 advanced tools giving your agents administration rights to manipulate chat rooms, govern users, and push automatic webhook notifications seamlessly.

### What you can do

- **Chatroom Moderation** — Let agents automatically mute misbehaving members out of massive chatrooms based on context
- **Identity Operations** — Ask the agent to block or generate users directly into your application cluster
- **Broadcasting & Support** — The LLM can send custom payload JSON objects or standard text messages to mobile peers seamlessly, without writing server-side REST configurations

### How it works

1. Sign up to the Netease Yunxin panel to acquire your AppKey and AppSecret.
2. Add them safely into Vurb.
3. The MCP translates native calls, building the complex `SHA1 Nonce` cryptographic checksum automatically.

### Who is this for?

- **Customer Service AI** — Proactive IM chat administration without manual intervention
- **Gaming Companies** — Integrate autonomous room administration for massively multiplayer rooms using Yunxin chat functionality


## Available Tools (11)
- **block_im_user**: Block an IM User network
- **create_chatroom**: Create a massive chatroom
- **create_im_user**: Create an IM User
- **destroy_chatroom**: Destroy a massive chatroom
- **get_chatroom_members**: Get Chatroom active members
- **mute_chatroom_member**: Mute a chatroom member
- **recall_message**: Recall a sent message
- **send_custom_message**: Send a Custom Payload Message
- **send_text_message**: Send a P2P Text Message
- **unblock_im_user**: Unblock an IM user
- **update_im_user**: Update an IM User profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Netease Yunxin IM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Mute the user 'spammer01' who is publishing spam in the chatroom '198273'. I am the operator 'admin01'."

**🤖 AI Agent:**
> User 'spammer01' has been definitively muted inside chatroom 198273 via the administrative endpoint. They can no longer send broadcast messages.

---

**👤 You:**
> "Send a text message saying 'Welcome back' from 'systemBot' to user 'john_doe'."

**🤖 AI Agent:**
> The message 'Welcome back' has been dispatched by `systemBot` asynchronously via the IM servers.


## ❓ FAQ

**Q: Is the cryptographic checksum handled locally?**
Yes! Netease API requires a very specific API Hash (Nonce + Secret + CurTime). This MCP server generates it securely on the fly so you just feed literal variables straight to the AI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netease-yunxin-im](https://vinkius.com/mcp/netease-yunxin-im)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Netease Yunxin IM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `netease-yunxin-im` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Netease Yunxin IM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "netease-yunxin-im": {
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
