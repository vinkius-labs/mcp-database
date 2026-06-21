# Cal.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calcom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/calcom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/calcom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage your scheduling via Cal.com — track bookings, manage event types, and coordinate meetings directly from any AI agent.

## Description
Connect your **Cal.com** account to any AI agent and orchestrate your scheduling, booking management, and availability through natural conversation.

### What you can do

- **Booking Oversight** — List all your bookings and retrieve detailed metadata, including attendee info and statuses.
- **Event Type Management** — List and retrieve detailed metadata for all your event types (templates).
- **Instant Scheduling** — Create new bookings directly from your workspace for specific event types and times.
- **Availability Coordination** — Access and monitor your schedules and memberships within organizations.
- **Booking Lifecycle** — Cancel existing bookings using natural language when plans change.
- **Account Insights** — Retrieve core profile information for the authenticated user.

### How it works

1. Subscribe to this server
2. Enter your Cal.com API Key and API Version
3. Start managing your calendar from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Busy Professionals** — quickly check for upcoming meetings or share booking links without manual calendar checking.
- **Sales & Success Teams** — retrieve event type details and coordinate with prospects straight from their workflow tools.
- **Developers** — integrate complex scheduling logic into their environment using natural language.


## Available Tools
- **cancel_booking**: This action cannot be undone.

Cancel an existing booking
- **create_booking**: The start time must be within an available slot.

Create a new booking on a specific event type
- **create_event_type**: Create a new event type (meeting template)
- **get_booking**: Get detailed information about a specific booking
- **get_event_type**: Get detailed configuration of a specific event type
- **get_current_user**: com profile information including name, email, timezone, and default schedule.

Retrieve the authenticated user profile
- **get_schedules**: Each event type references one schedule.

List all availability schedules
- **list_bookings**: Use to audit your calendar schedule.

List all bookings on your Cal.com account
- **list_event_types**: Use to discover bookable event types.

List all event types (meeting templates)
- **list_memberships**: List organization and team memberships


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cal.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming bookings in Cal.com."

**🤖 AI Agent:**
> I've retrieved your bookings. You have 3 upcoming meetings: 'Sync with Team' (ID: book_1), 'Intro Call' (ID: book_2), and 'Design Review' (ID: book_3).

---

**👤 You:**
> "Show the event types I have configured."

**🤖 AI Agent:**
> Retrieving event types... You have 3 templates: '15 Minute Meeting' (Slug: 15-min), '30 Minute Coffee' (Slug: coffee), and 'Full Audit' (Slug: audit).

---

**👤 You:**
> "Cancel booking with ID 99283."

**🤖 AI Agent:**
> Booking 99283 has been successfully cancelled in your Cal.com account. Notification emails have been sent to participants.


## Installation & Usage

To install and use the **Cal.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calcom](https://vinkius.com/mcp/calcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
