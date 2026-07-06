# Hathora MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hathora)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Orchestrate multiplayer game infrastructure via Hathora — manage applications, builds, deployments, and game rooms directly from your AI agent.

## Description
Connect your **Hathora** account to any AI agent and take full control of your multiplayer game server orchestration through natural conversation.

### What you can do

- **Application Management** — Create and inspect Hathora applications that represent your game services.
- **Build & Deployment** — Initiate new builds, upload server binaries, and configure deployments with specific CPU, memory, and environment variables.
- **Room Orchestration** — Spin up game rooms (sessions) across global regions (Seattle, London, Frankfurt, etc.) and retrieve connection info for clients.
- **Lobby Management** — Create public or private lobbies to facilitate player matchmaking and session discovery.
- **Process Monitoring** — List and monitor active server processes to keep track of your infrastructure's health.

### How it works

1. Subscribe to this server
2. Enter your Hathora Developer Token
3. Start managing your game infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — deploy new server versions and test room connectivity without leaving the code editor.
- **DevOps Engineers** — monitor active processes and manage global deployments through simple commands.
- **Studio Leads** — quickly check the status of game applications and infrastructure across different regions.


## Available Tools (9)
- **create_deployment**: Create a deployment for a build
- **create_lobby**: Create a new lobby
- **create_room**: Create a new game room (session)
- **get_application**: Get details for a specific Hathora application
- **get_room_connection_info**: Get connection info for a room
- **list_active_processes**: List active processes for an application
- **upload_build**: Upload a build file (tarball) for a specific build ID
- **create_application**: Create a new Hathora application
- **create_build**: Initiate a new build process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hathora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Hathora application named 'GalacticWarfare'."

**🤖 AI Agent:**
> I've created the application 'GalacticWarfare'. Its unique App ID is `app-789-xyz`. You can now use this ID to create builds and deployments.

---

**👤 You:**
> "Start a new game room for appId 'app-789-xyz' in the London region."

**🤖 AI Agent:**
> Requesting room creation in London... Success! Room `room-abc-123` is now active. Would you like the connection info for this room?

---

**👤 You:**
> "List all active processes for application 'app-789-xyz'."

**🤖 AI Agent:**
> I found 3 active processes for 'app-789-xyz'. Two are running in 'Seattle' and one in 'Frankfurt'. All processes are currently healthy.


## ❓ FAQ

**Q: How do I find the IP and port for players to connect to a specific game session?**
Use the `get_room_connection_info` tool with your App ID and Room ID. The agent will return the exact host and port details required for client-side connection.

**Q: Can I see how many server processes are currently running for my application?**
Yes! Run the `list_active_processes` action. It will provide a list of all active server processes associated with your specific Application ID.

**Q: How do I set up a matchmaking lobby for my game?**
You can use the `create_lobby` tool. You'll need to specify the App ID, visibility (public/private), and the region where the session should be hosted.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hathora](https://vinkius.com/mcp/hathora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hathora** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hathora` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hathora** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hathora": {
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
