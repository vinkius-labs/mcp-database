# OpenReplay MCP Server

Debug web applications by inspecting user sessions, technical events, and project data directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/openreplay)

## Overview
**Category:** developer-tools
**Tools Count:** 5

## Description
Connect your **OpenReplay** account to any AI agent to analyze user behavior and debug technical issues through natural conversation.

### What you can do

- **Project Overview** — List all projects associated with your account to quickly identify the environment you need to inspect.
- **Session Analysis** — Retrieve lists of user sessions for specific projects, with the ability to filter by User ID to track individual journeys.
- **Technical Deep-Dives** — Fetch detailed metadata and technical events (clicks, inputs, console logs) for any specific session to understand exactly what went wrong.
- **User Identification** — Search for specific users within your projects using emails or IDs to correlate support tickets with actual session recordings.

### How it works

1. Subscribe to this server
2. Enter your OpenReplay API Key
3. Start debugging and analyzing sessions from Claude, Cursor, or any MCP-compatible client

No more manually searching through session lists. Your AI acts as a support engineer or UX researcher, finding the exact technical context you need.

### Who is this for?

- **Support Engineers** — quickly find the session recording for a user reporting a bug without leaving the chat.
- **Developers** — inspect console logs and technical events directly from the code editor to reproduce issues faster.
- **Product Managers** — analyze user journeys and interactions to understand how features are being used in the wild.


## Available Tools
- **get_session**: Retrieve metadata for a single session
- **list_projects**: List all projects associated with your account
- **list_session_events**: ).

Retrieve all technical and user events recorded during a session
- **list_sessions**: Can filter by userId, limit, and page.

Retrieve a list of sessions for a specific project
- **search_users**: Find users identified within a project


## Installation & Usage

To install and use the **OpenReplay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openreplay](https://vinkius.com/mcp/openreplay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
