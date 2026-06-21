# Webex MCP Server

Manage rooms, meetings, and collaboration workflows on Cisco Webex — the leading enterprise video conferencing platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/webex)

## Overview
**Category:** industry-titans
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Webex** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webex](https://vinkius.com/mcp/webex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
