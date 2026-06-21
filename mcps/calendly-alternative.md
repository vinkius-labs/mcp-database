# Calendly MCP Server

Manage meetings and scheduling via Calendly — list event types, track scheduled events, inspect invitees and manage webhooks from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/calendly-alternative)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Connect your **Calendly** account to any AI agent and take full control of your scheduling operations through natural conversation.

### What you can do

- **Event Types** — List all meeting templates with their duration, type, description and scheduling URLs
- **Scheduled Events** — View upcoming and past meetings with invitee info, status and cancellation details
- **Invitee Management** — Browse attendees across all events with their names, emails and custom question responses
- **Availability** — Check user availability within a date range to find open slots before booking
- **Scheduling Links** — Create direct booking links for specific event types (no redirect needed)
- **Webhook Management** — List and create webhook subscriptions for event notifications (booking created, canceled, no-show)
- **Organization Memberships** — View team memberships and multi-user account structure

### How it works

1. Subscribe to this server
2. Enter your Calendly Personal Access Token
3. Start managing your calendar from Claude, Cursor, or any MCP-compatible client

No more switching to the Calendly app to check who booked what or review upcoming meetings. Your AI acts as a dedicated scheduling assistant.

### Who is this for?

- **Sales Teams** — quickly check upcoming meetings, review invitee details and track booking conversion rates
- **Developers** — create scheduling links programmatically, monitor webhook events and audit event type configurations
- **Managers** — review team availability, track meeting volume and manage webhook integrations via conversation


## Available Tools
- **create_scheduling_link**: Requires the event type URI and the owner type ("EventType" or "User"). Returns a booking URL that invitees can use to schedule a meeting directly via the API.

Create a scheduling link for direct booking
- **create_webhook**: Requires the callback URL, a list of events to subscribe to (e.g. ["invitee.created", "invitee.canceled", "invitee.no_show"]), and the scope (user or organization URI). Optionally provide a signing key for webhook verification.

Create a new webhook subscription in Calendly
- **get_event_type**: Provide the event type URI (found in list_event_types).

Get details for a specific Calendly event type
- **get_invitee**: Provide the invitee UUID from list_invitees.

Get details for a specific invitee
- **get_me**: Returns user ID, name, email, slug, organization URI, and scheduling URL. Use this to verify your token is working correctly and to get your user URI for filtering other queries.

Get the authenticated Calendly user
- **get_scheduled_event**: Provide the event UUID from list_scheduled_events.

Get details for a specific scheduled event
- **list_event_types**: Each event type includes its name, description, duration, type (one-on-one, group, collective, round_robin), scheduling URL, and active status. Optionally filter by a specific user URI. Use this to see what meeting options are available for booking.

List event types in Calendly
- **list_invitees**: Each invitee includes their name, email, event URI, scheduled start time, and responses to custom questions. Optionally filter by a specific event URI and set a count limit.

List invitees (attendees) across all Calendly events
- **list_memberships**: Each membership shows the user, organization, URI, and role. Useful for multi-team accounts and seeing which organizations you are part of.

List your memberships in Calendly organizations
- **list_scheduled_events**: Each event includes the event type, start time (UTC), invitee URI, status (active, canceled), and participants. Optionally filter by user URI, status (active or canceled), and count. Useful for reviewing your upcoming calendar.

List scheduled events (meetings) in Calendly
- **get_user_availability**: Requires the user URI, start time and end time (both ISO 8601 UTC format). Returns the user's scheduling rules, busy times, and date overrides. Useful for checking when someone is free before booking.

Get availability for a Calendly user
- **list_webhooks**: Each webhook shows its URL, scope (user or organization), subscribed events (invitee.created, invitee.canceled, etc.), and creation date. Use this to audit your event integrations.

List webhook subscriptions in Calendly


## Installation & Usage

To install and use the **Calendly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendly-alternative](https://vinkius.com/mcp/calendly-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
