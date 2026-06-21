# Microsoft Teams Events MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-teams-events)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Organize webinars and virtual events through Microsoft Teams with registration, attendee tracking, and engagement features.

## Description
Connect your **Microsoft Teams** account to any AI agent and take full control of your online meeting orchestration and automated collaboration workflows through natural conversation.

### What you can do

- **Meeting & Event Orchestration** â€” Programmatically create Teams meetings with unique join URLs and automated calendar synchronization
- **Attendee Intelligence** â€” List and manage your meeting participant directories, retrieving detailed attendance reports and interaction durations
- **Transcript & Recording Architecture** â€” Programmatically access text transcripts and recording metadata to maintain a perfectly coordinated audit trail of team discussions
- **Virtual Event Management** â€” Access and monitor specialized webinars and town halls to coordinate your large-scale organizational broadcasting
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor meeting volume directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** from the Microsoft Entra admin center (requires Microsoft Graph permissions)
3. Start orchestrating your Teams meetings from Claude, Cursor, or any MCP client

No more manual copy-pasting of meeting links or digging through chat history for transcripts. Your AI acts as your dedicated meeting coordinator and collaboration architect.

### Who is this for?

- **Project Managers** â€” instantly schedule team syncs and retrieve attendance reports using natural language commands
- **HR & Training Teams** â€” orchestrate internal webinars and verify participant engagement without leaving your creative workspace
- **Developers** â€” integrate high-speed Teams meeting data into custom internal tools through simple AI queries


## Available Tools (10)
- **cancel_event**: Cancel a calendar event
- **check_teams_status**: Verify Microsoft Graph API connectivity
- **create_meeting**: Pass attendee emails as comma-separated values.

Create a Teams meeting
- **get_attendance_report**: Get attendance report
- **get_event**: Get event details
- **get_profile**: Get user profile
- **get_webinar**: Get webinar details
- **list_events**: List calendar events
- **list_online_meetings**: List online meetings
- **list_webinars**: List webinars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft Teams Events** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Teams meeting with John and Sarah for tomorrow at 2pm."

**🤖 AI Agent:**
> Meeting created! Subject: 'Meeting with John & Sarah', tomorrow 2-3pm UTC. Teams link: https://teams.microsoft.com/l/... Both attendees have been invited. Would you like to add an agenda?

---

**👤 You:**
> "Show the attendance report for meeting MTG-2048."

**🤖 AI Agent:**
> Meeting MTG-2048 had 8 participants. 6 joined on time, 1 was 5 min late, and 1 left 10 min early. Average duration: 52 min. Would you like to export this data?

---

**👤 You:**
> "List all upcoming webinars."

**🤖 AI Agent:**
> You have 3 upcoming webinars. The next one is 'Q2 Product Launch' on May 5 with 142 registrants. Would you like to see registration details or session data?


## ❓ FAQ

**Q: How do I create a Teams meeting from my AI agent?**
Use the `create_meeting` tool with subject, start and end times (ISO 8601), and attendee emails. A Teams meeting link is generated automatically.

**Q: Can I check attendance after a meeting?**
Yes. Use `get_attendance_report` with the meeting ID to retrieve join/leave times for each participant.

**Q: Does this connector support webinars?**
Absolutely. Use `list_webinars` to see all scheduled webinars and `get_webinar` for detailed session and registration data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-teams-events](https://vinkius.com/mcp/microsoft-teams-events)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microsoft Teams Events** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microsoft-teams-events` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microsoft Teams Events** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microsoft-teams-events": {
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
