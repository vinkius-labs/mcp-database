# Cal.com MCP Server

Manage your scheduling via Cal.com — track bookings, manage event types, and coordinate meetings directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/calcom)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Cal.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calcom](https://vinkius.com/mcp/calcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
