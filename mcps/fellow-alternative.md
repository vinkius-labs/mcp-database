# Fellow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fellow-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fellow-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fellow-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Run better meetings with collaborative agendas, action item tracking, and AI-generated summaries that keep teams accountable.

## Description
Connect your **Fellow** workspace to any AI agent and manage your entire meeting workflow through natural conversation.

### What you can do

- **Meetings** — List and inspect meetings with titles, participants, dates, and agendas.
- **Notes** — Access structured meeting notes and AI-generated summaries.
- **Action Items** — Create, track, and complete action items with assignees and due dates.
- **Streams** — Browse recurring meeting series and their schedules.
- **Users** — List all workspace members and their roles.

### How it works

1. Subscribe to this server
2. Enter your Fellow API key (User Settings > Developer Tools)
3. Start managing meetings from Claude, Cursor, or any MCP client

### Who is this for?

- **Team Leads** — review meeting notes and action items without opening Fellow.
- **Project Managers** — track follow-up tasks and ensure accountability.
- **Remote Teams** — stay aligned on meeting outcomes and decisions.


## Available Tools
- **check_fellow_status**: Verify Fellow API connectivity
- **complete_action_item**: Mark an action item as completed
- **create_action_item**: Optionally link it to a meeting, assign to a user by email, and set a due date.

Create a new action item from a meeting
- **get_action_item**: Get details of a specific action item
- **get_meeting**: Get full details of a specific meeting
- **get_note**: Get full content of a specific note
- **get_stream**: Get details of a specific meeting stream
- **list_action_items**: Optionally filter by status: "pending", "completed", or "archived".

List action items from meetings
- **list_meetings**: List recent meetings from Fellow
- **list_notes**: Optionally filter by a specific meeting ID to get notes for that meeting only.

List meeting notes
- **list_streams**: List all meeting streams (recurring series)
- **list_users**: List all users in the Fellow workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fellow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my recent meetings in Fellow."

**🤖 AI Agent:**
> I found 5 recent meetings: 'Weekly Standup' (today 9:00 AM), 'Product Review' (yesterday 2:00 PM), 'Sprint Planning' (Monday 10:00 AM), '1:1 with Sarah' (last Friday), and 'Q3 Roadmap' (last Thursday). Want to see the notes for any of these?

---

**👤 You:**
> "Create an action item 'Send proposal to client' and assign it to sarah@team.com with a due date of May 10."

**🤖 AI Agent:**
> Done! Action item 'Send proposal to client' has been created and assigned to Sarah (sarah@team.com) with a due date of May 10, 2026.

---

**👤 You:**
> "List all pending action items."

**🤖 AI Agent:**
> You have 3 pending action items: 'Update API documentation' (due tomorrow, assigned to you), 'Review PR #542' (due Friday, assigned to Marcus), and 'Send proposal to client' (due May 10, assigned to Sarah). Want me to complete any of these?


## Installation & Usage

To install and use the **Fellow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fellow-alternative](https://vinkius.com/mcp/fellow-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
