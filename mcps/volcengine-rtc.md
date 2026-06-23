# Volcengine RTC MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/volcengine-rtc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Bring ByteDance's internal RTC Engine to your AI workflow. Administrate audio/video calls, manage servers, and start Mixes.

## Description
Empower your Agent with **Volcengine RTC**, the exact same Real-Time Communication backbone powering ByteDance's most prominent applications like TikTok and Douyin globally. This plugin provides 10 core administrative functions to manipulate streams autonomously.

### What you can do

- **Real-time Live Stream Operation** — Mute and unmute broadcaster audio/video feeds directly through natural language
- **Automated Expulsions** — Remove abusive streamers via Room ID controls dynamically
- **MCU Mixing & Recording** — Spin up cloud mixing or save streams directly to VOD storage effortlessly
- **Topology Oversight** — Query active servers, discover users inside those rooms and evaluate network drop rates

### How it works

1. Install this MCP server
2. Log into the Volcengine IAM Console to get an **Access Key (AK)** and **Secret Key (SK)**
3. Plug those alongside your **RTC App ID** into your client. The Vurb extension engine will dynamically convert the AI's natural language into signed HMAC-SHA256 REST API commands.

### Who is this for?

- **Stream Operators** — Command AI to instantly mute streamers acting inappropriately without fumbling through dashboards
- **Network Analysts** — Analyze dropped frame rates to determine poor connectivity in a specific node purely from prompt traces


## Available Tools (10)
- **get_active_rooms**: List all active RTC rooms in Volcengine
- **get_quality_metrics**: Get deep dive metrics of an RTC room
- **get_room_users**: Get list of users in a Volcengine room
- **kick_user**: Kick a user from a Volcengine RTC room
- **mute_stream**: StreamType should be "audio" or "video".

Mute a specific stream output (audio or video)
- **start_cloud_record**: Start Volcengine Cloud Recording
- **start_transcode**: Start Cloud MCU stream transcoding
- **stop_cloud_record**: Stop Volcengine Cloud Recording
- **stop_transcode**: Stop MCU stream transcoding
- **unmute_stream**: StreamType should be "audio" or "video".

Unmute a previously muted stream output


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Volcengine RTC** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Mute both audio and video streams for user 'player01' in room 'Squad_44'."

**🤖 AI Agent:**
> Sure. I executed a `MuteStream` command on Volcengine isolating user `player01`. Their stream is now blocked.

---

**👤 You:**
> "How many active sessions does my RTC App have right now?"

**🤖 AI Agent:**
> I queried the `ListRooms` API. There are currently 12 distinct rooms broadcasting, pulling a total of 58 users.


## ❓ FAQ

**Q: Does this support Volcengine HMAC-SHA256 V4 Signatures?**
Absolutely. Generating ByteDance's API signatures programmatically is challenging for raw agents. This backend completely conceals the cryptography layer so your agent can execute queries instantly just by having the Secret Key stored securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/volcengine-rtc](https://vinkius.com/mcp/volcengine-rtc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Volcengine RTC** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `volcengine-rtc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Volcengine RTC** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "volcengine-rtc": {
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
