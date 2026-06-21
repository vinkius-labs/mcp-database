# Venue MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/venue)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/venue-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/venue-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage event venues with booking calendars, client contracts, and catering coordination for wedding and conference spaces.

## Description
Connect your **Venue.live** account to any AI agent and simplify how you coordinate high-engagement virtual events, webinars, and interactive sessions through natural conversation.

### What you can do

- **Event Management** — List all upcoming webinars, create new events, and retrieve detailed configuration metadata.
- **Session Coordination** — List and manage individual sessions or breakout rooms associated with your events.
- **Speaker Registry** — Create and list guest speaker profiles to manage your event directory.
- **Attendee Tracking** — List registered participants for specific events to monitor growth and sign-ups.
- **Engagement Analytics** — Retrieve performance metrics and attendance data for completed events to measure success.
- **Recording Library** — List and access video recordings from past events for content repurposing.

### How it works

1. Subscribe to this server
2. Enter your Venue API Key (found in your workspace settings)
3. Start managing your virtual venue from Claude, Cursor, or any MCP client

### Who is this for?

- **Event Planners** — quickly retrieve speaker lists and session details via simple AI commands.
- **Marketing Managers** — monitor registration counts and check event analytics without leaving the workspace.
- **Community Leads** — automate the creation of new events and manage attendee lists directly via the AI assistant.


## Available Tools
- **create_event**: Create a new virtual event
- **create_speaker**: Register a new speaker
- **get_event_analytics**: Get event engagement analytics
- **get_event_details**: Get details of a specific event
- **get_me**: Get account information
- **list_events**: live.

List virtual events and webinars
- **list_recordings**: List event recordings
- **list_event_registrations**: List event attendees
- **list_event_sessions**: List sessions for a specific event
- **list_speakers**: List guest speakers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venue** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all upcoming events in my Venue account."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming sessions: 'Product Launch Keynote', 'User Feedback Webinar', and 'Q4 Strategy Review'. Which one would you like details on?

---

**👤 You:**
> "Show me the analytics for the 'Summer Webinar' (ID: ev_10293)."

**🤖 AI Agent:**
> Fetching analytics... The 'Summer Webinar' had 150 unique attendees with an average engagement time of 45 minutes. There were 25 questions asked in the chat. Shall I retrieve the attendee list?

---

**👤 You:**
> "Create a new event titled 'AI Workshop' for Dec 10th at 2 PM UTC."

**🤖 AI Agent:**
> Success! The 'AI Workshop' has been scheduled for 2024-12-10 at 14:00 UTC (ID: ev_8823). I've added the title and start time. Would you like to add a description or register a speaker now?


## Installation & Usage

To install and use the **Venue** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/venue](https://vinkius.com/mcp/venue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
