# Zoom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage video meetings, webinars, and users on Zoom — the world's leading collaboration and communication platform.

## Description
Connect your **Zoom** account to any AI agent and manage your video communication infrastructure through natural conversation.

### What you can do

- **Meeting Lifecycle** — Schedule new video meetings, retrieve full details (including join URLs), update topics, or cancel sessions directly from your agent
- **Webinar Management** — List all scheduled webinars, create new sessions, and retrieve deep metadata for attendee coordination
- **User discovery** — Browse and list all users in your Zoom account, and retrieve comprehensive profile details for specific team members
- **Deep Meeting Audit** — Retrieve real-time meeting statuses and join configurations to facilitate instant collaboration
- **Team Coordination** — Lookup host IDs and verify scheduled sessions across multiple users within your organization
- **Data Integrity** — Safely delete obsolete or cancelled meetings through simple chat commands to keep your calendar clean
- **Connectivity Health** — Verify your Zoom account configurations and available meeting features through automated metadata retrieval

### How it works

1. Subscribe to this server
2. Enter your Zoom OAuth Token
3. Start managing your meetings and webinars through Claude, Cursor, or any MCP-compatible client

No more manual navigation through complex meeting dashboards to find a join link. Your AI agent becomes your video communication coordinator.

### Who is this for?

- **Project Managers** — automate meeting creation for recurring syncs and coordinate team schedules through chat
- **Event Coordinators** — manage webinar schedules and retrieve attendee metadata without manual data entry
- **Executive Assistants** — quickly schedule or reschedule video meetings and verify join details for external partners
- **HR Managers** — lookup team member profiles and manage organizational user lists efficiently


## Available Tools
- **list_webinars**: List scheduled webinars
- **update_meeting**: Update meeting topic
- **get_meeting_participants**: List participants of a past meeting
- **delete_meeting**: Delete a meeting
- **create_meeting**: Create a video meeting
- **create_webinar**: Create a new webinar
- **get_meeting**: Get meeting details
- **get_recording**: Get recording files for a specific meeting
- **get_user**: Get user configuration
- **get_webinar**: Get webinar details
- **list_meetings**: List scheduled meetings
- **list_recordings**: List cloud recordings for a user
- **list_registrants**: List registrants for a meeting
- **list_users**: List Zoom users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zoom meetings for today."

**🤖 AI Agent:**
> I found 3 meetings scheduled for today: 1. 'Daily Standup' (ID: 12345), 2. 'Client Proposal' (ID: 67890), and 3. 'Engineering Sync' (ID: 11223). Which one would you like the join link for?

---

**👤 You:**
> "Schedule a meeting called 'Design Review' for 45 minutes."

**🤖 AI Agent:**
> Success! I've scheduled the 'Design Review' meeting. Duration: 45 minutes. Your Join URL is: https://zoom.us/j/123456789. Would you like me to add this to your meeting history list?

---

**👤 You:**
> "Show me the details for user 'me'."

**🤖 AI Agent:**
> Your Zoom Profile Details: Name: Alice Johnson, Email: alice@example.com, Account Type: Licensed (Pro), Personal Meeting ID: 123-456-7890. You currently have 5 active meetings scheduled.


## Installation & Usage

To install and use the **Zoom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoom](https://vinkius.com/mcp/zoom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
