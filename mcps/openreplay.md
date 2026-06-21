# OpenReplay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openreplay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Debug web applications by inspecting user sessions, technical events, and project data directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenReplay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all projects in my OpenReplay account."

**🤖 AI Agent:**
> I've found 3 projects: 'Main Web App' (ID: 12), 'Mobile Dashboard' (ID: 45), and 'Staging Environment' (ID: 8). Which one would you like to explore?

---

**👤 You:**
> "Find the last 5 sessions for user 'john@example.com' in project 12."

**🤖 AI Agent:**
> Searching for the user... Found User ID 'user_99'. Here are the 5 most recent sessions for John, including a 12-minute session from today at 10:30 AM. Would you like to see the events for that session?

---

**👤 You:**
> "Show me any console errors or clicks for session ID 'sess-abc-123'."

**🤖 AI Agent:**
> Inspecting session 'sess-abc-123'... I found a 'Uncaught TypeError' at 02:15 and a series of rapid clicks on the 'Submit' button immediately following the error. It looks like a validation issue.


## ❓ FAQ

**Q: Can I see technical logs and console errors for a specific session?**
Yes! Use the `list_session_events` tool with a Session ID. It will retrieve all recorded technical and user events, including clicks, inputs, and console logs.

**Q: How do I find sessions for a specific user email?**
First, use `search_users` with the email and Project ID to find the user. Then, use `list_sessions` with that User ID to see all their recorded activity.

**Q: Does this integration support self-hosted OpenReplay instances?**
Yes. You can provide an optional `OPENREPLAY_BASE_URL` during setup to point the agent to your private instance instead of the default cloud API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openreplay](https://vinkius.com/mcp/openreplay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenReplay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `openreplay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenReplay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openreplay": {
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
