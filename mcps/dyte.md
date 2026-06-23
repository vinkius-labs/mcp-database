# Dyte MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dyte)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage live video and audio experiences via Dyte — create meetings, manage participants, and control recordings or livestreams directly from any AI agent.

## Description
Connect your **Dyte** organization to any AI agent to orchestrate real-time communication workflows. From spinning up instant meeting rooms to managing complex recording and livestreaming configurations, your AI acts as a powerful backend controller for your video infrastructure.

### What you can do

- **Meeting Orchestration** — Create, list, and retrieve details for video meetings instantly using `create_meeting` and `list_meetings`.
- **Participant Management** — Add users to meetings via `add_participant` and generate the required auth tokens for your frontend SDKs.
- **Recording Control** — Start and stop recordings with custom storage configurations (like AWS S3) and fetch download URLs using `get_recording`.
- **Livestreaming** — Broadcast your meetings to wider audiences with simple `start_livestream` and `stop_livestream` commands.
- **Webhooks** — Configure real-time event notifications for your server using `create_webhook` to stay updated on meeting starts and ends.

### How it works

1. Subscribe to this server
2. Enter your Dyte Organization ID and API Key
3. Start managing your video infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate and test video workflows without writing boilerplate code or using external API clients.
- **Product Managers** — monitor active meetings, list participants, and manage recording assets directly through conversation.
- **Operations Teams** — automate meeting creation and participant access for webinars, interviews, or internal calls.


## Available Tools (11)
- **add_participant**: Add a participant to a meeting
- **create_meeting**: Create a new Dyte meeting
- **create_webhook**: Create a webhook
- **get_meeting**: Fetch meeting details
- **get_recording**: Fetch recording details
- **list_meetings**: Fetch all meetings
- **list_participants**: Fetch participants in a meeting
- **start_livestream**: Start livestreaming for a meeting
- **start_recording**: Optionally accepts storage configuration.

Start recording a meeting
- **stop_livestream**: Stop the active livestream for a meeting
- **stop_recording**: Stop an active recording


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dyte** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Dyte meeting titled 'Product Strategy Sync' in the ap-south-1 region."

**🤖 AI Agent:**
> I've created the meeting 'Product Strategy Sync'. The Meeting ID is `7b2a...`. You can now add participants or start the session.

---

**👤 You:**
> "Add a participant named 'Alice Smith' to meeting 7b2a... using the 'group_call_host' preset."

**🤖 AI Agent:**
> Alice Smith has been added to the meeting. Here is the auth token for the frontend: `eyJhbG...`.

---

**👤 You:**
> "Start recording for meeting 7b2a... and list all current participants."

**🤖 AI Agent:**
> Recording has started for meeting 7b2a... (Recording ID: `rec_123`). Currently, there are 3 participants: Alice Smith, Bob Jones, and Charlie Brown.


## ❓ FAQ

**Q: How do I get the authentication token for a new participant to join a meeting?**
Use the `add_participant` tool. You need to provide the `meeting_id`, `name`, and a `preset_name`. The tool will return the `authToken` required by Dyte's frontend SDKs.

**Q: Can I configure where my meeting recordings are stored?**
Yes. When using the `start_recording` tool, you can optionally provide a `storage_config` JSON object (e.g., for AWS S3) to define your custom storage destination.

**Q: How can I monitor when a meeting starts or ends in real-time?**
You can use the `create_webhook` tool to register a URL that Dyte will notify when specific events occur, such as `meeting.started` or `meeting.ended`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dyte](https://vinkius.com/mcp/dyte)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dyte** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dyte` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dyte** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dyte": {
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
