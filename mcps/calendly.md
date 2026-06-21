# Calendly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calendly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/calendly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/calendly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate scheduling workflows via Calendly — manage event types, scheduled events, invitees, and availability directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What meetings do I have scheduled for tomorrow?"

**🤖 AI Agent:**
> You have 3 meetings tomorrow. 09:00 — Product Demo with Sarah Chen (30 min). 11:00 — Sales Discovery with James Park (45 min). 14:30 — Onboarding Call with Maria Lopez (60 min). Would you like me to pull the invitee details for any of them?

---

**👤 You:**
> "How many no-shows did we have this week?"

**🤖 AI Agent:**
> 4 no-shows this week across 28 scheduled events (14.3% rate). Highest concentration on Monday — 2 missed Discovery Calls. The invitees were notified but did not join. I can mark them as no-shows and pull their contact details for follow-up.

---

**👤 You:**
> "Am I free on Friday afternoon for a 30-minute call?"

**🤖 AI Agent:**
> Checking your availability… You have a free slot from 15:00 to 16:30 on Friday. Your 30-Minute Meeting event type is active and has availability in that window. Would you like me to share your scheduling link, or should I create a one-off event?


## Installation & Usage

To install and use the **Calendly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendly](https://vinkius.com/mcp/calendly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
