# GoTo Meeting MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goto-meeting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/goto-meeting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/goto-meeting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Host reliable video conferences with screen sharing, recording, and transcription for productive remote team meetings.

## Description
Connect your **GoTo Meeting** account to any AI agent and manage your video conferencing workflow through natural conversation.

### What you can do

- **Meeting Scheduling** — Create new meetings with subject, start time, end time, and meeting type (immediate, scheduled, or recurring)
- **Upcoming Meetings** — List all scheduled meetings with connection links and attendee details
- **Meeting Details** — Inspect individual meeting configurations, connection URLs, and settings
- **Meeting History** — Browse past meetings with duration, start times, and attendance records
- **Meeting Cancellation** — Delete scheduled meetings that are no longer needed
- **Organizer Management** — List all meeting organizers configured in your organization

### How it works

1. Subscribe to this server
2. Enter your GoTo Meeting OAuth Access Token
3. Start managing your meetings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Executive Assistants** — schedule, review, and manage meetings without switching to the GoTo Meeting dashboard
- **Team Leads** — check upcoming meetings, cancel sessions, and manage organizer accounts
- **Operations Teams** — audit meeting history, track usage patterns, and manage scheduling through AI


## Available Tools
- **create_meeting**: Schedule a new meeting
- **delete_meeting**: Delete a meeting
- **get_meeting_details**: Get details for a specific meeting
- **list_meeting_history**: List historical meetings
- **list_meetings**: List upcoming GoTo Meeting sessions
- **list_account_organizers**: List account organizers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoTo Meeting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Schedule a meeting titled 'Q2 Planning Review' for next Tuesday from 2 PM to 3 PM."

**🤖 AI Agent:**
> Meeting scheduled! Subject: 'Q2 Planning Review'. Date: Tuesday, April 29, 2025. Time: 2:00 PM – 3:00 PM (EST). Meeting ID: mtg_29401. Join URL: https://goto.com/meeting/29401. Dial-in: +1 (872) 240-3212, Access Code: 291-847-205. Type: scheduled. The meeting is now visible in your upcoming meetings list. Would you like to view all upcoming meetings or create another?

---

**👤 You:**
> "Show all my upcoming meetings this week and cancel the one on Friday."

**🤖 AI Agent:**
> You have 4 upcoming meetings this week: 1) 'Sprint Standup' — Mon 9:00 AM (mtg_29380, recurring). 2) 'Client Demo — Apex Corp' — Tue 11:00 AM (mtg_29392). 3) 'Q2 Planning Review' — Tue 2:00 PM (mtg_29401). 4) 'Weekly Sync' — Fri 10:00 AM (mtg_29415). Canceling 'Weekly Sync' (mtg_29415)... ✅ Meeting deleted successfully. You now have 3 meetings remaining this week. Would you like to see the meeting history or check organizer details?

---

**👤 You:**
> "Show me the meeting history from last month and list all organizers in our account."

**🤖 AI Agent:**
> Last month's meeting history: 47 meetings held. Total duration: 62 hours 15 minutes. Average meeting length: 1h 19m. Most active day: Wednesday (14 meetings). Longest meeting: 'Board Review Q1' (3h 12m, 12 attendees). Organizers in your account: 1) Sarah Chen (sarah@company.com, Admin). 2) Mike Torres (mike@company.com, Organizer). 3) Lisa Park (lisa@company.com, Organizer). 4) API Bot (bot@company.com, Organizer). Would you like to schedule a new meeting or check details for a specific past session?


## Installation & Usage

To install and use the **GoTo Meeting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goto-meeting](https://vinkius.com/mcp/goto-meeting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
