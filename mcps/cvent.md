# Cvent MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cvent)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cvent-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cvent-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage event registrations, sessions, and attendees directly via the Cvent API.

## Description
Integrate **Cvent**, the world's leading event management platform, directly into your AI workflow. Manage your large-scale conferences, meetings, and seminars, track attendee lists, and monitor event sessions using natural language.

### What you can do

- **Event Oversight** — List and retrieve full details for all your upcoming and past events managed in Cvent.
- **Attendee Management** — Quickly access registration lists and individual attendee profiles for specific events.
- **Session & Speaker Tracking** — Monitor scheduled sessions and associated speakers across your event portfolio.
- **Venue Discovery** — List and explore venues configured in your account for event planning.

### How it works

1. Connect the Cvent integration to your AI assistant.
2. Authorize using your Cvent Client ID and Client Secret (found in the Cvent Developer Portal).
3. Manage your event lifecycle through intuitive conversation.

### Who is this for?

- **Conference Organizers** — Quickly check registration numbers and session details on the go.
- **Event Planners** — Access venue and speaker information directly via chat during planning sessions.
- **Operations Teams** — Monitor attendee lists and event statuses across large-scale portfolios.


## Available Tools
- **get_account_details**: Resolves account identifiers and organizational settings. Interacts with the account configuration boundary.

Retrieve metadata for your Cvent account
- **get_event_details**: Resolves event configuration, capacity, and lifecycle status. Touches the granular event planning and operational boundary.

Get detailed information for a specific event
- **list_active_events**: Resolves operational event records. Touches the event status management boundary.

Quickly list only the events that are currently active
- **list_event_attendees**: Resolves attendee identifiers and registration status. Touches the registration and participant management boundary.

List all registered attendees for a specific event
- **list_events**: Resolves event IDs, titles, start/end dates, and current status. Interacts with the core event management boundary.

List all events in your Cvent account
- **list_registration_types**: Resolves registration type identifiers and names. Interacts with the registration logic and pricing boundary.

List available registration types for an event
- **list_event_sessions**: Resolves session IDs, titles, and time slots. Touches the agenda and session scheduling boundary.

List all sessions scheduled for an event
- **list_event_speakers**: Resolves speaker names and biographies. Interacts with the speaker management and content boundary.

List speakers associated with an event
- **list_available_venues**: Resolves venue IDs, names, and address metadata. Touches the venue and logistics boundary.

List venues configured in the account
- **search_events_by_filter**: Resolves matching event records. Touches the indexed event search boundary.

Search for events using a filter string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cvent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events in my Cvent account."

**🤖 AI Agent:**
> I've found 3 active events: 'Annual Global Summit', 'Q3 Sales Kickoff', and 'Product Launch 2024'. Would you like to see the registration status for any of these?

---

**👤 You:**
> "Show me the speakers for the 'Annual Global Summit' event."

**🤖 AI Agent:**
> The 'Annual Global Summit' (ID: 123) has 12 speakers confirmed, including 'Dr. Aris Thorne' and 'Sarah Jenkins'. Should I list their session assignments?

---

**👤 You:**
> "Who is registered for the 'Q3 Sales Kickoff' event?"

**🤖 AI Agent:**
> There are currently 45 people registered for 'Q3 Sales Kickoff'. 30 have completed their registration, and 15 are pending. Would you like to see the list of pending attendees?


## Installation & Usage

To install and use the **Cvent** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cvent](https://vinkius.com/mcp/cvent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
