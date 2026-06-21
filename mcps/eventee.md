# Eventee MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventee)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventee-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventee-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage events, track speakers, and monitor attendee engagement via the Eventee API.

## Description
Integrate **Eventee**, the leading mobile-first event management platform, directly into your AI workflow. Manage your event schedules and sessions, track registered speakers and attendees, monitor audience questions and partner sponsorships, and oversee your event engagement using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, dates, and status for all your Eventee projects.
- **Speaker & Session Intelligence** — Monitor event schedules, resolving session titles, speaker bios, and unique identifiers.
- **Engagement Management** — Access and monitor audience questions and attendee registration progress in real-time.
- **Event Auditing** — Retrieve high-level summaries of session volume, speaker diversity, and organizational event health instantly.

### How it works

1. Connect the Eventee integration to your AI assistant.
2. Authorize using your Eventee API Key (found in your account settings).
3. Orchestrate your event planning and mobile engagement strategy through intuitive conversation.

### Who is this for?

- **Event Planners** — Quickly check session schedules and speaker details on the go.
- **Marketing Teams** — Research attendee engagement and partner visibility via chat during live events.
- **Operations Teams** — Monitor registration counts and organizational event metadata instantly.


## Available Tools
- **get_eventee_account_metadata**: Retrieve metadata and limits for your Eventee account
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **quick_event_engagement_audit**: Retrieve a high-level summary of sessions, speakers, and attendees
- **list_currently_active_events**: Identify events that are currently taking place
- **list_event_registered_attendees**: List all registered attendees for a specific event
- **list_all_events**: List all events managed in your Eventee account
- **list_event_partners_and_sponsors**: List all partners and sponsors for a specific event
- **list_event_audience_questions**: List all questions submitted by the audience for a specific event
- **list_event_sessions**: List all sessions and schedule items for a specific event
- **list_event_speakers**: List all speakers registered for a specific event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all sessions for event ID 'EVENT-12345'."

**🤖 AI Agent:**
> I've found 12 sessions for event 'EVENT-12345', including 'Opening Keynote' (10:00 AM) and 'Product Deep Dive' (2:00 PM). Would you like to see the speakers for the Keynote?

---

**👤 You:**
> "What audience questions have been submitted for today's event?"

**🤖 AI Agent:**
> For today's event, 5 questions have been submitted, including 'How does the new API handle scale?' and 'What is the release date?'. 3 questions are currently awaiting moderation. Should I pull the session IDs they are associated with?

---

**👤 You:**
> "Show me the sponsors for our upcoming conference."

**🤖 AI Agent:**
> I've retrieved 8 partners/sponsors for the upcoming conference, including 'TechCorp' (Platinum), 'InnoVentures' (Gold), and 'Global Solutions'. Would you like the contact information for TechCorp?


## Installation & Usage

To install and use the **Eventee** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventee](https://vinkius.com/mcp/eventee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
