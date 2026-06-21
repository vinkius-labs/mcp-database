# Hathora MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hathora)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hathora-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hathora-mcp)
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


## Available Tools
- **create_application**: Create a new Hathora application
- **create_build**: Initiate a new build process
- **create_deployment**: Create a deployment for a build
- **create_lobby**: Create a new lobby
- **create_room**: Create a new game room (session)
- **get_application**: Get details for a specific Hathora application
- **get_room_connection_info**: Get connection info for a room
- **list_active_processes**: List active processes for an application
- **upload_build**: Upload a build file (tarball) for a specific build ID


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


## Installation & Usage

To install and use the **Hathora** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hathora](https://vinkius.com/mcp/hathora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
