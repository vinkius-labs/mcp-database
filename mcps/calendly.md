# Calendly MCP Server

Automate scheduling workflows via Calendly — manage event types, scheduled events, invitees, and availability directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/calendly)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Calendly** account to any AI agent and take full control of your scheduling workflow through natural conversation.

### What you can do

- **Event Types** — List, create, and manage your event types with custom durations, locations, and availability rules
- **Scheduled Events** — Browse upcoming and past events, view attendee details, and check event status
- **Invitees** — List invitees for any event, view their responses, UTM parameters, and tracking data
- **Availability** — Check your real-time availability and manage scheduling windows
- **Users & Organization** — View your profile, organization membership, and team structure
- **Cancellations & No-Shows** — Track cancellations with reasons and mark invitees as no-shows for accurate reporting

### How it works

1. Subscribe to this server
2. Enter your Calendly Personal Access Token
3. Start managing your schedule from Claude, Cursor, or any MCP-compatible client

No more switching between your calendar app and your workspace. Your AI agent becomes your scheduling command center.

### Who is this for?

- **Sales teams** — review upcoming demos, check invitee details, and prepare for calls without leaving your CRM workflow
- **Recruiters** — manage interview schedules and track candidate attendance across multiple event types
- **Customer success managers** — monitor onboarding calls, follow up on no-shows, and analyze meeting patterns
- **Founders & executives** — get a quick summary of your week's meetings and availability gaps


## Available Tools
- **get_user**: Get the authenticated Calendly user profile including name, email, timezone, avatar URL, scheduling URL, organization URI, and current plan
- **list_event_types**: List all event types configured for a Calendly user (meeting templates)
- **get_event_type**: Retrieve detailed configuration for a specific Calendly event type by UUID
- **list_scheduled_events**: List all scheduled events (past or upcoming) for a Calendly user
- **get_scheduled_event**: Get full details of a specific scheduled Calendly event by tracking UUID
- **list_invitees**: List all invitees/attendees for a specific Calendly scheduled event
- **cancel_event**: Cancel a scheduled Calendly event with an optional cancellation reason sent to the invitee
- **list_availability**: Retrieve all availability schedules configured for a Calendly user
- **get_available_times**: Get available booking time slots for a specific Calendly event type within an explicit date range
- **list_org_members**: List all members of the Calendly organization retrieving team structures


## Installation & Usage

To install and use the **Calendly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendly](https://vinkius.com/mcp/calendly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
