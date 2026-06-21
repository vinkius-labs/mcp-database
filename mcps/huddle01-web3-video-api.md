# Huddle01 (Web3 Video API) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/huddle01-web3-video-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/huddle01-web3-video-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/huddle01-web3-video-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Build and manage Web3 video meetings with Huddle01 — create rooms, track live sessions, and retrieve meeting recordings directly from your AI agent.

## Description
Connect the power of **Huddle01's Web3 Video SDK** to your AI agent. This server allows you to orchestrate decentralized communication infrastructure through simple natural language commands.

### What you can do

- **Room Management** — Create new meeting rooms with specific configurations (locked/unlocked) and custom metadata using `create_room` and `get_rooms`.
- **Live Session Monitoring** — Track active meetings in real-time, check peer counts, and list current participants with `get_live_sessions` and `get_live_session_participants`.
- **Historical Data** — Retrieve past session details, participant lists, and meeting metadata using `get_room_sessions` and `get_participant_list`.
- **Recordings & Metrics** — Access meeting recordings via `get_recordings` and monitor your API usage statistics with `get_metrics`.

### How it works

1. Subscribe to this server
2. Enter your Huddle01 API Key from the developer dashboard
3. Start managing your video infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web3 Developers** — Integrate video meeting management directly into your development workflow or DAO tooling.
- **Community Managers** — Monitor live community calls and retrieve participant lists for attendance tracking without leaving your chat interface.
- **Product Teams** — Automate the creation of meeting rooms and track platform usage metrics through conversational AI.


## Available Tools
- **create_room**: You must specify if the room is locked.

Create a new Huddle01 meeting room
- **get_live_session_details**: Fetch details of a specific active room
- **get_live_session_participants**: Fetch participants currently present in a live room
- **get_live_sessions**: Fetch rooms that are currently active
- **get_metrics**: Fetch usage statistics for your API key
- **get_participant_list**: Retrieve participants who joined a specific session
- **get_recordings**: Can be filtered by sessionId.

Fetch recordings created using the SDK
- **get_room_details**: Retrieve information about a specific room
- **get_room_metadata**: Retrieve only the metadata for a specific room
- **get_room_sessions**: Retrieve all sessions (meetings) held in a specific room
- **get_rooms**: Fetch all rooms associated with your API key


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Huddle01 (Web3 Video API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new locked Huddle01 room for our private team sync."

**🤖 AI Agent:**
> I've created a new locked room for you. The Room ID is 'abc-123-xyz'. You can now share this ID with your team.

---

**👤 You:**
> "Show me all currently active live sessions and how many people are in them."

**🤖 AI Agent:**
> Fetching live sessions... I found 2 active rooms. Room 'room-A' has 5 participants, and Room 'room-B' has 12 participants.

---

**👤 You:**
> "List the recordings available for session ID 'sess-9988'."

**🤖 AI Agent:**
> I found one recording for session 'sess-9988'. You can access it at the following URL: [Recording Link].


## Installation & Usage

To install and use the **Huddle01 (Web3 Video API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/huddle01-web3-video-api](https://vinkius.com/mcp/huddle01-web3-video-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
