# EventMobi MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventmobi)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventmobi-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventmobi-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deliver immersive event experiences with virtual and hybrid event tools, networking features, and live engagement analytics.

## Description
Connect your **EventMobi** Experience Manager account to any AI agent and take full control of your conference logistics and attendee engagement workflows through natural conversation.

### What you can do

- **Event Orchestration** — List and manage multiple events programmatically, including retrieving detailed metadata about branding and settings
- **Agenda Architecture** — Access complete event schedules and session tracks to maintain a high-fidelity record of workshops and presentations
- **Attendee Lifecycle** — Programmatically register new participants and manage check-ins for specific sessions to streamline event entry
- **Engagement Intelligence** — Monitor live polls and gamification challenges directly through your agent to track real-time attendee participation
- **Operational Monitoring** — Manage real-time data sync webhooks and retrieve participant directories to maintain a perfectly coordinated event ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the EventMobi Experience Manager (Integrations tab)
3. Start managing your conference engagement from Claude, Cursor, or any MCP client

No more manual session updates or complex attendee lookups. Your AI acts as your dedicated conference strategist and engagement coordinator.

### Who is this for?

- **Conference Planners** — instantly update agenda details and monitor session check-ins using natural language commands
- **Marketing Teams** — track poll results and gamification leaderboards without leaving your workspace
- **Operations Leads** — automate attendee registration and manage data sync webhooks through simple AI queries


## Available Tools
- **attendee_checkin**: Check in an attendee
- **register_attendee**: Create a new attendee profile
- **create_agenda_session**: Add a new session to the agenda
- **create_webhook**: Subscribe to event triggers
- **get_event_details**: Get metadata for an event
- **list_gamification_challenges**: List gamification challenges
- **list_events**: List all managed events
- **list_attendees**: List event participants (attendees)
- **list_live_polls**: List event polls
- **list_sessions**: List event agenda sessions
- **list_event_tracks**: List session tracks
- **list_webhooks**: List event webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EventMobi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events in EventMobi."

**🤖 AI Agent:**
> I've retrieved your events. You have 2 active gatherings: 'Global Sales Kickoff' (ID: em_123) and 'Partner Summit'. Which one should I provide the attendee list for?

---

**👤 You:**
> "Show the agenda for 'Global Sales Kickoff' (ID: em_123)."

**🤖 AI Agent:**
> Fetching agenda for em_123... I found 8 scheduled sessions, including 'Product Vision 2026' and 'Sales Strategy'. Would you like to check the track categories for these sessions?

---

**👤 You:**
> "Check in attendee ID 'p_456' for the 'Product Vision' session."

**🤖 AI Agent:**
> Action complete! Attendee p_456 has been successfully checked in for the 'Product Vision' session. The arrival is now logged in your EventMobi analytics.


## Installation & Usage

To install and use the **EventMobi** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventmobi](https://vinkius.com/mcp/eventmobi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
