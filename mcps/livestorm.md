# Livestorm MCP Server

Connect your AI agent to Livestorm to manage webinars, registrations, attendees, and analytics via natural language.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/livestorm)

## Overview
**Category:** video-conferencing
**Tools Count:** 10

## Description
Integrate **Livestorm**, the leading browser-based webinar and video events platform, directly into your AI workflow. Manage webinar schedules, track registrations, monitor attendee engagement, access real-time analytics, and send replay emails — all through conversational AI.

### What you can do

- **Webinar Management** — List, create, and retrieve all your webinars with scheduling and status information
- **Registration Tracking** — View all registrations for any webinar, create new attendee registrations, and verify individual registration details
- **Attendee Monitoring** — List attendees who actually joined events, track attendance duration and engagement metrics
- **Analytics & Reporting** — Access post-event analytics including registration counts, attendance rates, and replay views
- **Replay Distribution** — Send replay email links to all attendees of completed events with one action
- **Room Management** — List all webinar rooms in your Livestorm workspace for infrastructure planning

### How it works

1. Connect the Livestorm integration to your AI assistant
2. Authorize using your Livestorm API Token (found in Settings → Integrations → API)
3. Manage your webinar ecosystem and track engagement through intuitive conversation

### Who is this for?

- **Marketing Teams** — Monitor registration growth, track attendance rates, and send replay campaigns
- **Event Planners** — Create and manage webinars, verify attendee lists, and audit event health
- **Sales Teams** — Identify engaged attendees and follow up with prospects who attended your product demos
- **Customer Success** — Track training webinar attendance and send replay links to customers who missed sessions


## Available Tools
- **create_event**: Provide at minimum the event title. Optionally specify description, start/end times, and event type (live, replay, or on-demand).

Create a new webinar or event in Livestorm
- **create_registration**: Creates a new registration record for the specified webinar. The registration email must be unique for that webinar.

Register a new attendee for a Livestorm webinar
- **get_event**: Use list_events first to find the correct ID. Returns full event metadata including settings, registration page URL, and status.

Retrieve detailed information for a specific Livestorm webinar or event
- **get_registration**: Returns the full registration record for the specified attendee.

Retrieve details for a specific registration of a Livestorm webinar
- **list_analytics**: Returns registration counts, attendance rates, replay views, and engagement metrics. Useful for post-event reporting and ROI analysis.

Retrieve analytics data for a specific Livestorm webinar
- **list_attendees**: Returns only attendees who joined the event, not just registered attendees. Includes attendance duration and engagement data.

Retrieve the list of attendees who actually attended a Livestorm webinar
- **list_events**: Returns all events (live, replay, scheduled).

Retrieve a list of all webinars and events in your Livestorm account
- **list_registrations**: Returns attendee details including names, emails, and registration status. Useful for verifying attendance lists.

Retrieve all registrations for a specific Livestorm webinar
- **list_webinar_rooms**: Useful for understanding your Livestorm workspace structure.

Retrieve a list of all rooms (webinar rooms) in your Livestorm workspace
- **send_replay**: Sends the replay link to everyone who attended the specified event. Use after live events to share the recording with attendees.

Send a replay email to all attendees of a completed Livestorm webinar


## Installation & Usage

To install and use the **Livestorm** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/livestorm](https://vinkius.com/mcp/livestorm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
