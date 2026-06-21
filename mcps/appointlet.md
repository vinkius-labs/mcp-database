# Appointlet MCP Server

Bring Appointlet scheduling directly into your AI agent — list schedules, track bookings, cancel events, and manage attendees seamlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/appointlet)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Appointlet** scheduling workspace to any AI agent to streamline booking operations, access client intake forms, and orchestrate meeting lifecycles directly via natural language. Forget jumping through tabs and let your virtual agent manage your calendar logistics.

### What you can do

- **Scheduling Pages** — Retrieve all available booking links and overall configurations for your account
- **Meeting Types** — Pull details on available meeting formats, including durations, conferencing tools, and status
- **Booking Operations** — Discover scheduled meetings, access filled intake forms, or instantly cancel a booking with a custom reason
- **Team Availability** — List members assigned to different scheduling pages to audit round-robin workloads
- **Organization Stats** — Audit the Appointlet workspace status, tier, and connected members

### How it works

1. Subscribe to this server
2. Insert your Appointlet API Key
3. Start querying your weekly meetings from Claude, Cursor, or any MCP ecosystem app

### Who is this for?

- **Sales Development Reps** — fetch custom intake field responses for your upcoming discovery calls instantly
- **Support Leaders** — audit team distribution and list active user availability on your scheduling pages
- **Consultants** — command the AI to list today's bookings and quickly cancel/reschedule with a written prompt if an emergency strikes
- **Account Managers** — review historical tracking data and client responses to prep for follow-ups


## Available Tools
- **list_scheduling_pages**: Each page has a unique booking URL.

List all scheduling pages in the Appointlet organization
- **get_scheduling_page**: Retrieve detailed information for a specific Appointlet scheduling page
- **list_meeting_types**: List all meeting types configured for an Appointlet scheduling page
- **get_meeting_type**: Get detailed configuration for a specific Appointlet meeting type
- **list_bookings**: Useful for reporting and CRM sync.

List all bookings for an Appointlet scheduling page
- **get_booking**: Get full details of a specific Appointlet booking
- **cancel_booking**: The attendee receives a cancellation notification email. The time slot becomes available for new bookings.

Cancel an existing Appointlet booking
- **list_members**: Members receive meetings via round-robin or pooled availability.

List all team members assigned to an Appointlet scheduling page
- **get_organization**: The organization is the top-level account entity.

Get the Appointlet organization profile
- **list_intake_fields**: Returns field names, types, and required status.

List all custom intake form fields for an Appointlet meeting type


## Installation & Usage

To install and use the **Appointlet** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appointlet](https://vinkius.com/mcp/appointlet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
