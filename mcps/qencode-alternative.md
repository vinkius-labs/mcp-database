# Qencode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qencode-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate video transcoding and live streaming via Qencode — manage tasks, start encodings, and orchestrate live streams directly from any AI agent.

## Description
Connect your **Qencode** account to any AI agent to handle high-performance video processing and live broadcasting through natural conversation.

### What you can do

- **Video Transcoding** — Initialize tasks and start encoding processes with custom JSON queries for source and output formats
- **Live Streaming** — Create and manage live streams using RTMP, WebRTC, or SRT protocols with HLS/CMAF delivery
- **Simulcasting** — Add restreaming targets like YouTube or Twitch to your active live feeds automatically
- **Status Monitoring** — Track the real-time progress of multiple transcoding tasks (downloading, encoding, saving)
- **Infrastructure Management** — Manage custom CDN domains and update live stream configurations like DVR settings

### How it works

1. Subscribe to this server
2. Enter your Qencode API Key
3. Start processing video assets and managing broadcasts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Video Engineers** — automate complex transcoding workflows and monitor task queues without leaving the terminal or editor
- **Content Platforms** — orchestrate live streaming infrastructure and simulcasting targets programmatically
- **Product Teams** — integrate video processing status checks directly into project management or dev tools


## Available Tools
- **add_simulcast_target**: Add a simulcast target to a live stream
- **create_domain**: Create a custom CDN domain
- **create_live_stream**: Requires a live access token.

Create a new live stream
- **create_task**: Create a new transcoding task
- **get_access_token**: Required before creating tasks.

Get a session-based access token for transcoding
- **get_live_access_token**: Get an access token for live streaming
- **get_task_status**: Get the status of one or more transcoding tasks
- **start_encode**: Start a transcoding task with specific parameters
- **start_live_stream**: Start a live stream
- **stop_live_stream**: Stop a live stream
- **update_live_stream**: Update a live stream configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Qencode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a session access token for transcoding."

**🤖 AI Agent:**
> I've retrieved your session token. You can now use it to initialize new transcoding tasks.

---

**👤 You:**
> "Check the status of task tokens 550e8400-e29b and 660f9500-f30c."

**🤖 AI Agent:**
> Task 550e8400-e29b is currently 'encoding' (45% complete), while task 660f9500-f30c has 'completed' successfully.

---

**👤 You:**
> "Create a new live stream named 'Webinar' with RTMP input and HLS output."

**🤖 AI Agent:**
> Live stream 'Webinar' has been created. Stream ID: st_98234. You can now start the stream using the `start_live_stream` tool.


## ❓ FAQ

**Q: How can I check if my video is finished encoding?**
Use the `get_task_status` tool with your task tokens. It returns the current state such as 'downloading', 'encoding', 'saving', or 'completed' for one or more tasks.

**Q: Can I stream to multiple platforms like YouTube and Twitch at once?**
Yes! First create a stream with `create_live_stream`, then use `add_simulcast_target` to add external destinations to your live feed.

**Q: Do I need to get an access token before every transcoding task?**
Yes, you must call `get_access_token` to receive a session-based token required by the `create_task` tool. For live streaming, use `get_live_access_token` instead.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qencode-alternative](https://vinkius.com/mcp/qencode-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Qencode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `qencode-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Qencode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qencode-alternative": {
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
