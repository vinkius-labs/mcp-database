# Eventtia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventtia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventtia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventtia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Equip your AI agent to manage events, track B2B meetings, and monitor attendee data via the Eventtia API.

## Description
Integrate **Eventtia**, the all-in-one event management platform, directly into your AI workflow. Manage your corporate events and conferences, track registered attendees and speaker profiles, monitor session schedules and B2B business meetings, and oversee your event engagement using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, venues, and status for all your Eventtia projects.
- **Attendee Intelligence** — Monitor participant profiles, resolving professional categories, emails, and unique identifiers.
- **Meeting Management** — Access and monitor B2B business meetings and networking pairings to stay ahead of participant interaction.
- **Event Auditing** — Retrieve high-level summaries of attendee volume, session activity, and organizational event health instantly.

### How it works

1. Connect the Eventtia integration to your AI assistant.
2. Authorize using your Eventtia API Key (found in your account settings).
3. Orchestrate your event planning and business networking strategy through intuitive conversation.

### Who is this for?

- **Corporate Event Planners** — Quickly check attendee counts and session schedules on the go.
- **B2B Matchmaking Leads** — Research business meeting pairs and networking status via chat during live events.
- **Operations Teams** — Monitor registration progress and organizational event metadata instantly.


## Available Tools
- **get_eventtia_account_metadata**: Retrieve metadata and limits for your Eventtia account
- **get_event_performance_stats**: Get high-level performance metrics for a specific event
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **quick_event_engagement_audit**: Retrieve a high-level summary of attendees, sessions, and meetings
- **list_currently_live_events**: Identify events that are currently active or ongoing
- **list_event_attendees**: List all registered attendees for a specific event
- **list_event_business_meetings**: List all B2B networking and business meetings for a specific event
- **list_all_events**: List all events managed in your Eventtia account
- **list_event_sessions**: List all sessions and schedule items for a specific event
- **list_event_speakers**: List all speakers registered for a specific event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventtia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active conferences."

**🤖 AI Agent:**
> I've found 3 active conferences, including 'Global Tech Expo' and 'B2B Sales Summit'. The Tech Expo currently has 850 registered attendees. Would you like to see the meeting schedule for this event?

---

**👤 You:**
> "Show me the business meetings for event ID '12345'."

**🤖 AI Agent:**
> For event ID '12345', I've retrieved 45 scheduled business meetings, including pairings between 'TechCorp' and 'Innovation Lab'. 15 meetings are currently in progress. Should I pull the participant roles for these meetings?

---

**👤 You:**
> "Search for attendees matching 'Sarah' in the Sales Summit."

**🤖 AI Agent:**
> I've found 3 attendees matching 'Sarah': 'Sarah Miller' (VP Sales), 'Sarah Connor' (Business Analyst), and 'Sarah Williams'. All are registered for the main conference. Would you like the profile details for Sarah Miller?


## Installation & Usage

To install and use the **Eventtia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventtia](https://vinkius.com/mcp/eventtia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
