# Netease Yunxin IM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netease-yunxin-im)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/netease-yunxin-im-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/netease-yunxin-im-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Netease Yunxin IM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netease-yunxin-im](https://vinkius.com/mcp/netease-yunxin-im)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
