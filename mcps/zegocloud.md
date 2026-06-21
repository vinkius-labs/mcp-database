# ZegoCloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zegocloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zegocloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zegocloud-mcp)
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


## Installation & Usage

To install and use the **ZegoCloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zegocloud](https://vinkius.com/mcp/zegocloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
