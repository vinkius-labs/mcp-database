# join.me MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/joinme)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Start instant video meetings with screen sharing and recording that works in the browser with no downloads required.

## Description
Connect your **join.me** account to any AI agent and manage video meetings through natural conversation.

### What you can do

- **Meeting Scheduling** — Create, update, and cancel meetings with customizable settings
- **Participant Management** — Invite participants, track attendance, and manage access
- **Recording Access** — List and retrieve meeting recordings
- **Meeting History** — Browse past meetings with duration and participant data
- **Settings Configuration** — Manage account and meeting preferences

### How it works

1. Subscribe to this server
2. Enter your join.me Access Token
3. Start managing meetings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Teams** — schedule meetings and manage invites through AI
- **Managers** — review meeting history and recording availability
- **Assistants** — coordinate calendars and meeting logistics


## Available Tools
- **create_webhook**: Register a new webhook
- **delete_meeting**: Cancel/Delete a meeting
- **get_meeting**: Get details of a specific meeting
- **get_user_info**: me user profile.

Get account information
- **list_meetings**: me account.

List your join.me meetings
- **list_webhooks**: me account.

List registered webhooks
- **schedule_meeting**: Schedule a future meeting
- **start_adhoc_meeting**: Start an instant meeting
- **start_scheduled_meeting**: Start a scheduled meeting
- **update_meeting**: Update a scheduled meeting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **join.me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Schedule a team standup for tomorrow at 9 AM and invite the engineering team."

**🤖 AI Agent:**
> Meeting scheduled! 'Engineering Standup'. Date: Apr 27, 9:00 AM (30 min). Participants: 6 invited (sarah@co.com, mike@co.com, lisa@co.com, james@co.com, chen@co.com, david@co.com). Join link: https://join.me/mtg-4521. Status: Confirmed. Invites sent. Would you like to add a recurring schedule or view today's meetings?

---

**👤 You:**
> "Show this week's meeting history and list available recordings."

**🤖 AI Agent:**
> This week: 12 meetings. Total time: 8h 45m. Average duration: 44 min. Largest: 'Quarterly Review' (90 min, 15 participants). Recordings: 4 available. 1) 'Quarterly Review' (90 min, 245 MB). 2) 'Client Demo' (45 min, 120 MB). 3) 'Design Review' (60 min, 180 MB). 4) 'Sprint Retro' (30 min, 80 MB).

---

**👤 You:**
> "Cancel tomorrow's 3 PM meeting and update the standup to 9:30 AM."

**🤖 AI Agent:**
> Cancelled: 'Budget Review' (Apr 27, 3:00 PM). All 4 participants notified. Updated: 'Engineering Standup' moved to 9:30 AM. All 6 participants notified of time change. Tomorrow's schedule: 9:30 AM Standup (30 min), 11:00 AM Client Call (60 min), 2:00 PM Design Review (45 min).


## ❓ FAQ

**Q: Can I schedule meetings and invite participants?**
Yes. Create meetings with date, time, duration, and participant list. Update existing meetings and cancel when needed. Each meeting generates a join link for easy sharing.

**Q: Can I access meeting recordings?**
Yes. List all available recordings and retrieve download links. Recordings include meeting metadata, duration, and participant information.

**Q: Can I view past meeting history and attendance?**
Yes. Browse meeting history with details including duration, participant count, attendees, and whether the meeting was recorded.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/joinme](https://vinkius.com/mcp/joinme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **join.me** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `joinme` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **join.me** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "joinme": {
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
