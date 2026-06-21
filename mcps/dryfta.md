# Dryfta MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dryfta)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/dryfta-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/dryfta-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage event attendees, track sessions, and monitor abstract submissions via the Dryfta API.

## Description
Integrate **Dryfta**, the all-in-one event management platform, directly into your AI workflow. Manage your event attendees and registration statuses, track scheduled sessions and speaker assignments, monitor abstract submissions and review cycles, and oversee your event exhibitors using natural language.

### What you can do

- **Attendee Oversight** — List and retrieve detailed information and registration status for all your event participants.
- **Program Intelligence** — Monitor event sessions, workshops, speaker profiles, and real-time venue assignments.
- **Abstract Management** — Track submitted abstracts for your call for papers, including authors and current review statuses.
- **Exhibitor Monitoring** — List all event exhibitors and sponsors, resolving booth assignments and sponsorship levels.

### How it works

1. Connect the Dryfta integration to your AI assistant.
2. Authorize using your Dryfta subdomain and API Key.
3. Orchestrate your event planning and attendee management through intuitive conversation.

### Who is this for?

- **Event Managers** — Quickly check registration volumes and session schedules on the go.
- **Program Chairs** — Monitor abstract submission progress and review statuses via chat.
- **Operations Teams** — Research specific attendee details and exhibitor assignments instantly.


## Available Tools
- **get_dryfta_account_metadata**: Retrieve metadata and limits for your Dryfta account
- **get_attendee_details**: Get detailed profile and registration status for a specific attendee
- **quick_event_enrollment_audit**: Retrieve a high-level summary of attendee registration volumes
- **get_session_details**: Get detailed information and speaker list for a specific session
- **list_submitted_abstracts**: List all abstracts submitted for the event (call for papers)
- **list_event_attendees**: List all attendees registered for your Dryfta event
- **list_event_exhibitors**: List all exhibitors and sponsors registered for the event
- **list_event_sessions**: List all scheduled sessions and workshops in the event program
- **list_upcoming_sessions**: Identify sessions that are scheduled to start soon (mock logic)
- **search_attendees_by_keyword**: Search for attendees using a name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dryfta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all registered attendees for our conference."

**🤖 AI Agent:**
> I've found several registered attendees, including 'Alice Johnson' (Standard) and 'Bob Miller' (VIP). Would you like to see the contact details for any of these participants?

---

**👤 You:**
> "Show me the sessions scheduled for tomorrow."

**🤖 AI Agent:**
> Tomorrow's sessions include 'AI in Healthcare' at 10:00 AM (Room A) and 'Future of MCP' at 2:00 PM (Main Hall). Should I pull the speaker list for the AI session?

---

**👤 You:**
> "Check the status of submitted abstracts."

**🤖 AI Agent:**
> I've retrieved 12 submitted abstracts. 5 are 'Under Review', 3 are 'Accepted', and 4 are 'Pending'. Would you like a list of the accepted abstract titles?


## Installation & Usage

To install and use the **Dryfta** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dryfta](https://vinkius.com/mcp/dryfta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
