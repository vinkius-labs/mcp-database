# Webex MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webex)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/webex-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/webex-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage rooms, meetings, and collaboration workflows on Cisco Webex — the leading enterprise video conferencing platform.

## Description
Connect your **Cisco Webex** account to any AI agent and manage your enterprise collaboration through natural conversation.

### What you can do

- **Space Management** — List all Webex rooms (spaces) you belong to and create new collaboration areas with ease
- **Meeting Lifecycle** — Schedule new video meetings, update existing schedules, or cancel sessions directly from your agent
- **Collaboration Insights** — Retrieve full details for rooms and meetings, including join URLs, dial-in numbers, and precise timing
- **Team Organization** — Rename existing spaces or permanently delete obsolete rooms to keep your workspace organized
- **Deep Discovery** — Quickly find unique room and meeting UUIDs required for automated collaboration workflows
- **Real-Time Auditing** — Monitor your calendar for upcoming scheduled meetings and verify your participation status

### How it works

1. Subscribe to this server
2. Enter your Webex Personal Access Token
3. Start managing your rooms and meetings through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex meeting dashboards to find a join link. Your AI agent becomes your collaboration coordinator.

### Who is this for?

- **Project Managers** — automate space creation for new projects and coordinate meeting schedules through chat
- **Enterprise Teams** — quickly find join links and meeting details for upcoming internal or external sessions
- **DevOps Engineers** — automate collaboration room provisioning and manage meeting lifecycle for incident response
- **Executive Assistants** — schedule and reschedule video meetings and verify space history with simple commands


## Available Tools
- **create_video_meeting**: Provide a title and ISO 8601 start/end timestamps.

Schedules a new Webex video meeting
- **create_webex_room**: Provide a descriptive title for the room.

Creates a new Webex space
- **delete_scheduled_meeting**: This action is irreversible.

Permanently cancels and deletes a scheduled Webex meeting
- **delete_webex_room**: This action is irreversible and removes all history for the room.

Permanently deletes a Webex room
- **get_meeting_details**: Retrieves details for a specific Webex meeting
- **get_room_details**: Retrieves details for a specific Webex room
- **list_scheduled_meetings**: Lists scheduled Webex meetings
- **list_webex_rooms**: Lists all Webex rooms (spaces) the authenticated user belongs to
- **update_meeting_schedule**: Provide the meeting ID and the updated fields.

Updates the time or title of an existing Webex meeting
- **update_room_title**: Provide the room ID and the new title.

Updates the title of an existing Webex room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Webex rooms."

**🤖 AI Agent:**
> I found 5 rooms you belong to: 'Project Phoenix', 'Engineering Daily', 'Marketing Sync', 'General Space', and 'Incident Response'. Which one would you like to see details for?

---

**👤 You:**
> "Schedule a meeting called 'Q1 Strategy' for tomorrow from 10:00 to 11:00 AM."

**🤖 AI Agent:**
> Success! I've scheduled the 'Q1 Strategy' meeting (ID: mtg-abc) for 2026-04-01 from 10:00 AM to 11:00 AM. I can provide the join link whenever you're ready.

---

**👤 You:**
> "What meetings do I have scheduled for today?"

**🤖 AI Agent:**
> Searching your Webex calendar… You have 2 meetings today: 1. 'Daily Standup' at 09:30 AM and 2. 'Client Review' at 02:00 PM. Would you like the join details for either of these?


## Installation & Usage

To install and use the **Webex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webex](https://vinkius.com/mcp/webex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
