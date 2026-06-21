# Truto Unified Calendar MCP Server

Empower your AI agent with a universal API to read, schedule, and sync events seamlessly across Google, Outlook, and other major calendar providers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/truto-unified-calendar)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Deploy the ultimate scheduling machine by linking your AI agent to **Truto**. Instead of building fragmented code for individual calendar APIs, Truto provides a normalized schema that controls Google Calendar, Outlook, and countless others underneath. Command your agent to list daily events, find free timeslots accurately, or write absolute meetings directly to the chosen provider without swapping logic loops.

### What you can do

- **Unified Calendar Tracking** — Check all connected calendars regardless of provider natively and list their available events continuously
- **Meeting Generation** — Instruct your AI to generate or directly cancel/update specific events passing ISO-compliant timings directly to the root provider
- **Free/Busy Analysis** — Demand explicit gaps inside your schedule bypassing complex metadata just extracting readable unavailable/available blocks
- **Integration Audit** — Check the absolute status of all connected root provider connections (Integrations) to ensure nothing is decoupled abruptly
- **Event Forensics** — Interrogate and extract any granular metadata embedded inside an `event_id`, including conferencing details and attendee lists

### How it works

1. Anchor this multi-calendar instance to your local Vinkius conversational agent
2. Provide the Master Token from Truto combined specifically with your `Integrated Account ID` targeting a specific linked provider
3. Engage scheduling queries organically conversing with your assistant

### Who is this for?

- **Executive Assistants** — Book multi-provider meetings strictly through conversational commands checking calendar gaps dynamically
- **Sales Coordinators** — Force event creation securely across varied client infrastructures without logging into fragmented Google and Microsoft portals
- **Platform Architects** — Centralize routing logic manipulating the agent to alter calendar entries strictly using one unified schema rule


## Available Tools
- **create_event**: Provide calendar_id, title, and start/end times in ISO format.

Create a new event in a calendar via Truto. The event is written through to the underlying provider (Google/Outlook) in real-time. Provide calendar ID, title, and ISO 8601 start/end times
- **delete_event**: This action is irreversible.

Delete an event via Truto. The event is removed from both Truto and the underlying provider in real-time
- **get_calendar**: Get details of a specific calendar via Truto by ID. Returns calendar name, provider, timezone, and metadata normalized to the Truto unified schema
- **get_event**: Get full details of a specific event via Truto. Returns title, description, start/end times, attendees, location, organizer, recurrence, and provider-specific metadata
- **get_free_busy**: Provide calendar_id and time range.

Get free/busy data for a calendar via Truto within a date range. Returns time blocks as free or busy in the unified Truto format
- **list_calendars**: List all calendars via Truto unified API. Truto provides a real-time, pass-through API that normalizes calendar data across Google Calendar, Outlook Calendar, and other providers into a consistent schema
- **list_connections**: List all integrated accounts (connections) in Truto. Shows connected calendar providers, auth status, and account metadata
- **list_events**: Provide the calendar_id.

List all events from a calendar via Truto. Returns events in a unified format regardless of the underlying provider. Shows titles, times, attendees, locations, and conferencing info
- **update_event**: Provide the event_id and a JSON updates object.

Update an existing event via Truto. Provide a JSON object with fields to change. Changes pass through to the real provider in real-time
- **validate_connection**: Validate a Truto integrated account connection. Checks credentials, permissions, and API accessibility. Returns validation status and any errors


## Installation & Usage

To install and use the **Truto Unified Calendar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truto-unified-calendar](https://vinkius.com/mcp/truto-unified-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
