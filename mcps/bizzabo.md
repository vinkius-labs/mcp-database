# Bizzabo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bizzabo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bizzabo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bizzabo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate your event experience via Bizzabo — manage events, registrations, and attendees directly from any AI agent.

## Description
Connect your **Bizzabo** account to any AI agent and orchestrate your events, registrations, and attendee workflows through natural conversation.

### What you can do

- **Event Oversight** — List and retrieve detailed information for all your upcoming and past events.
- **Registration Tracking** — Query and monitor event registrations to track ticket sales and attendee growth.
- **Contact Management** — Access your directory of attendees, speakers, and exhibitors across all events.
- **Session & Speaker Coordination** — Retrieve schedules and speaker details to ensure your event runs smoothly.
- **Ticket Type Discovery** — List available registration types and form properties for specific events.

### How it works

1. Subscribe to this server
2. Enter your Bizzabo API Key
3. Start managing your events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Planners** — quickly check registration counts and event details without opening the dashboard.
- **Marketing Teams** — retrieve attendee lists and metadata straight from their workflow tools.
- **Ops Teams** — monitor session schedules and speaker details using natural language.


## Available Tools
- **get_contact**: Get specific contact details
- **get_event**: Get specific event details
- **get_registration**: Get specific registration details
- **get_session**: Get details of a specific session
- **list_contacts**: List all contacts across events
- **list_events**: List all Bizzabo events
- **list_registration_types**: List ticket types for an event
- **list_registrations**: List registrants for a specific event
- **list_sessions**: List sessions for an event
- **list_speakers**: List speakers for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bizzabo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events in Bizzabo."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming events: 'Annual Conference 2024' (ID: ev_1), 'Tech Summit' (ID: ev_2), and 'Developer Meetup' (ID: ev_3).

---

**👤 You:**
> "Show the sessions for event ev_1."

**🤖 AI Agent:**
> Retrieving sessions... I found 5 sessions, including 'Keynote: Future of Events', 'Panel: Digital Transformation', and 'Workshop: Networking Skills'. Which one would you like more details on?

---

**👤 You:**
> "Find the registration details for ID reg_992."

**🤖 AI Agent:**
> Registration reg_992 belongs to John Doe (john@example.com). They registered for the 'Early Bird' ticket type on March 15th and the status is 'Approved'.


## Installation & Usage

To install and use the **Bizzabo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bizzabo](https://vinkius.com/mcp/bizzabo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
