# MeetingPulse MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meetingpulse)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/meetingpulse-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/meetingpulse-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Interactive audience engagement via MeetingPulse — track polls, Q&As, and meeting analytics.

## Description
Connect your **MeetingPulse** account to any AI agent and take full control of your audience engagement and meeting data through natural conversation.

### What you can do

- **Meeting Oversight** — List all active and past meetings and fetch detailed configuration and status
- **Poll Monitoring** — Retrieve poll results, individual questions, and survey summaries in real-time
- **Engagement Analytics** — Access meeting engagement metrics and participant analytics instantly
- **Interaction Tracking** — Monitor Q&A sessions and list attendees for specific meetings
- **Resource Management** — List files and materials shared during your interactive sessions

### How it works

1. Subscribe to this server
2. Enter your MeetingPulse API Key
3. Start managing your audience engagement from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_account_info**: Get account information
- **get_meeting**: Get details for a specific meeting
- **get_meeting_analytics**: Get meeting analytics
- **get_poll_details**: Get details for a specific poll
- **list_attendees**: List meeting attendees
- **list_meeting_files**: List files shared in a meeting
- **list_meetings**: List all meetings
- **list_polls**: List polls for a meeting
- **list_qa_sessions**: List Q&A sessions
- **search_meetings**: Search meetings by term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MeetingPulse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active meetings in MeetingPulse."

**🤖 AI Agent:**
> Retrieving meetings... I found 2 active sessions: 'Product Launch 2024' and 'Weekly All-Hands'.

---

**👤 You:**
> "Show results for the poll 'Favorite Feature' in meeting ID 123."

**🤖 AI Agent:**
> Fetching poll data... The 'Favorite Feature' poll has 50 responses. 'AI Assistant' is leading with 60% of the votes.

---

**👤 You:**
> "Get engagement analytics for meeting ID 123."

**🤖 AI Agent:**
> Querying analytics... Meeting 123 had a 95% engagement rate with 120 questions asked in the Q&A session.


## Installation & Usage

To install and use the **MeetingPulse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meetingpulse](https://vinkius.com/mcp/meetingpulse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
