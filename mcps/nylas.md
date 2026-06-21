# Nylas MCP Server

Equip your AI agent to manage emails, calendars, and contacts across all providers (Gmail, Outlook) through a single unified interaction.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nylas)

## Overview
**Category:** talk-to-me
**Tools Count:** 10

## Description
Connect your **Nylas** account to your AI agent and seamlessly interact with communication data across 100% of email and calendar providers.

### What you can do

- **Email Management** — Use `list_messages` to read inbound emails, navigate through `list_folders` and `list_drafts`, or actively compose and dispatch emails live using `send_message`.
- **Calendar Syncing** — Fetch meeting tracking arrays via `list_calendars` and `list_events`, or actively block out new times by invoking `create_event`.
- **Contact Organization** — Rapidly enumerate directory users with `list_contacts` and insert newly met stakeholders via `create_contact` natively.

### How it works

1. Subscribe to this server
2. Enter your Nylas API Key (v3)
3. Start managing your cross-provider email and calendar architecture using Claude, Cursor, or your preferred AI client

### Who is this for?

- **Sales Development Reps** — automate email drafting, verify outbound calendar slots, and log contact information in seconds.
- **Founders & Executives** — triage the morning inbox securely, block out focus time on the calendar, and schedule meetings conversationally.
- **HR & Recruiting** — track candidate communications effectively and seamlessly schedule multi-party interviews directly from the terminal.


## Available Tools
- **list_calendars**: Returns internal calendar UUIDs required to execute event queries.

List all user calendars connected via Nylas
- **list_events**: List scheduled events mapped inside a specific Calendar UUID
- **create_event**: g. Google Calendar).

Create a new synchronized calendar event
- **delete_event**: Delete a specific calendar event from the provider
- **list_messages**: Retrieve the unified inbox/messages stream for the authenticated grant
- **send_message**: Dispatch an outbound email utilizing the native mail provider
- **list_contacts**: List natively synced address book contacts from the user account
- **create_contact**: Insert a brand new address book contact record
- **list_folders**: Enumerate the organizational email directories tracking labels/files
- **list_drafts**: Dump unsent email threads parked in the Drafts bound location


## Installation & Usage

To install and use the **Nylas** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nylas](https://vinkius.com/mcp/nylas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
