# RongCloud MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rongcloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Leading IM and RTC platform in China — manage users, messages, and chatrooms via AI.

## Description
Empower your AI agent to orchestrate your communication infrastructure with **RongCloud** (融云), the dominant IM and RTC platform in China. By connecting RongCloud to your agent, you transform complex user management, real-time messaging, and chatroom control into a natural conversation. Your agent can instantly retrieve connection tokens for users, monitor online status, send private or chatroom messages, and manage user blocks or blacklists without you ever needing to navigate the RongCloud Developer Console. Whether you are building a high-volume social app or coordinating enterprise communication, your agent acts as a real-time messaging assistant, keeping your communication flow accurate and your user data secure.

### What you can do

- **User Orchestration** — Retrieve IM tokens, refresh user profiles, and monitor real-time online status.
- **Messaging Control** — Send 1-to-1 private messages or broadcast messages to entire chatrooms.
- **Room Management** — Create and query chatrooms to coordinate group interactions.
- **Moderation & Security** — Manage blocked users and blacklists to maintain a healthy communication environment.
- **System Auditing** — Retrieve high-level information about your communication agents and active sessions.

### How it works

1. Subscribe to this server
2. Enter your RongCloud App Key and App Secret
3. Start managing your communication infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor user activity and coordinate feature releases through natural language queries.
- **Community Moderators** — manage user behavior and moderate chatroom content directly from your AI-powered workspace.
- **DevOps Engineers** — monitor system health and audit connection histories via a unified AI interface.
- **RongCloud Power Users** — integrate your existing communication workflows into your AI-driven daily routines.


## Available Tools (10)
- **check_online**: Check user online status
- **create_chatroom**: Create chatrooms
- **get_token**: Get user IM token
- **list_blacklist**: List user blacklist
- **list_blocked_users**: List blocked users
- **query_chatroom**: Get chatroom details
- **refresh_user**: Update user information
- **send_chatroom_msg**: Send chatroom message
- **send_private_msg**: Send private message
- **block_user**: Block user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RongCloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get an IM token for user 'mario-123'."

**🤖 AI Agent:**
> I've retrieved the connection token for Mario. You can use this token to initialize the client SDK for this user session.

---

**👤 You:**
> "Check if user 'renato-456' is currently online."

**🤖 AI Agent:**
> I've checked the status for Renato. He is currently 'Online' and connected to the IM server.

---

**👤 You:**
> "Send a text message to chatroom 'room-8821' from user 'bot-01'."

**🤖 AI Agent:**
> Done! I've sent your message to all participants in chatroom 'room-8821'. The message has been successfully broadcasted.


## ❓ FAQ

**Q: How do I find my RongCloud App Key and Secret?**
Log in to the RongCloud Developer Console, navigate to [Application Identification] or [Secret Management], and you will find your App Key and App Secret there. Note that Development and Production environments have separate keys.

**Q: Can I check if a user is currently online?**
Yes. Use the `check_online` tool with a user ID to retrieve their current connection status to the IM server.

**Q: Is it possible to manage chatrooms through this server?**
Yes! You can use the `create_chatroom` tool to initiate new rooms and `query_chatroom` to retrieve detailed information about existing ones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rongcloud](https://vinkius.com/mcp/rongcloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RongCloud** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rongcloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RongCloud** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rongcloud": {
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
