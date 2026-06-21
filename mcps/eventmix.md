# Eventmix MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventmix)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventmix-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventmix-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize events with integrated registration, payment processing, and attendee communication for conferences and meetups.

## Description
Connect your **Eventmix** account to any AI agent and take full control of your virtual event management and attendee engagement workflows through natural conversation.

### What you can do

- **Event Orchestration** — List and manage virtual events programmatically, including retrieving detailed metadata and updating event settings in real-time
- **Attendee & RSVP Management** — Register new participants and submit RSVPs for specific events to maintain high-fidelity attendance records
- **Schedule Intelligence** — Access event agendas and session schedules programmatically to keep your participants updated on the latest content
- **Engagement Analytics** — Retrieve detailed usage and engagement metrics for your virtual events to monitor performance and ROI directly through your agent
- **Operational Monitoring** — Check API connectivity and manage registration workflows (including codes) directly through your agent for reliable event operations

### How it works

1. Subscribe to this server
2. Retrieve your **X-API-Key** from your Eventmix dashboard (Account Settings > API)
3. Start managing your virtual events from Claude, Cursor, or any MCP client

No more manual attendee tracking or complex agenda navigation. Your AI acts as your dedicated virtual event and engagement coordinator.

### Who is this for?

- **Event Organizers** — instantly check registration counts and update session details using natural language queries
- **Marketing Teams** — monitor attendee engagement and manage registration codes without leaving your workspace
- **Community Managers** — keep members updated on event schedules and manage RSVPs through simple AI commands


## Available Tools
- **check_api_connectivity**: Verify Eventmix API status
- **create_new_event**: Requires a title and scheduled date.

Create a new virtual event
- **remove_virtual_event**: Delete a virtual event
- **get_event_usage_analytics**: Get analytics for an event
- **get_event_details**: Get details for a specific event
- **get_current_user_profile**: Get authenticated organization info
- **get_event_schedule**: Get the agenda/schedule for an event
- **list_event_attendees**: List participants for an event
- **list_virtual_events**: List all virtual events
- **submit_event_rsvp**: RSVP to a virtual event
- **send_registration_code**: Email a registration code
- **update_event_settings**: Modify an existing event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventmix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming virtual events on Eventmix."

**🤖 AI Agent:**
> I've retrieved your upcoming virtual events. You have 3 gatherings scheduled, including 'AI Product Summit' (ID: ev_123) and 'Growth Lab'. Would you like the agenda details for any of these?

---

**👤 You:**
> "Show me the attendee list for event ID 'ev_123'."

**🤖 AI Agent:**
> Fetching participants for event ev_123... I found 45 registered attendees. Notable participants include 'John Doe' and 'Jane Smith'. I can provide individual registration metadata if needed.

---

**👤 You:**
> "What is the engagement analytics for my latest event?"

**🤖 AI Agent:**
> Scanning analytics... Your latest virtual event had a total of 150 unique viewers with an average duration of 45 minutes per attendee. Engagement peaked during the 'Q&A' session. Shall I check for poll results?


## Installation & Usage

To install and use the **Eventmix** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventmix](https://vinkius.com/mcp/eventmix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
