# Calendly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calendly-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage meetings and scheduling via Calendly — list event types, track scheduled events, inspect invitees and manage webhooks from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calendly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my upcoming meetings this week."

**🤖 AI Agent:**
> I found 5 active scheduled events: 'Product Demo' with john@company.com (tomorrow at 14:00 UTC), '1:1 with Sarah' (Wednesday at 10:00 UTC), 'Team Standup' (Thursday at 09:00 UTC), 'Client Onboarding' (Thursday at 15:30 UTC) and 'Design Review' (Friday at 11:00 UTC).

---

**👤 You:**
> "What event types do I have available for booking?"

**🤖 AI Agent:**
> You have 4 active event types: '30 Minute Meeting' (one-on-one, 30 min), 'Product Demo' (one-on-one, 60 min), 'Team Sync' (group, 45 min, up to 6 people) and 'Office Hours' (collective, 30 min). Would you like the scheduling URL for any of these?

---

**👤 You:**
> "Create a direct scheduling link for my 30 Minute Meeting event type."

**🤖 AI Agent:**
> Done! I've created a scheduling link for your '30 Minute Meeting' event type. The URL is https://calendly.com/schedule/abc123xyz. Anyone with this link can book a 30-minute slot directly without going through the Calendly website.


## ❓ FAQ

**Q: How do I create a Calendly Personal Access Token?**
Log in to the [**Calendly Dashboard**](https://calendly.com), go to **Integrations & Settings > API & Webhooks**, and generate a Personal Access Token. Copy the token immediately — it won't be shown again.

**Q: Can I see who booked a meeting?**
Yes! Use `list_invitees` to see all attendees across your events, or `list_scheduled_events` to see upcoming meetings with their invitee URIs. Then use `get_invitee` with the invitee UUID to get their full name, email, timezone and answers to custom questions.

**Q: Can I check availability before booking?**
Yes! Use `get_user_availability` with the user's URI, start time and end time (ISO 8601 UTC). It returns the user's scheduling rules, busy times and date overrides so you can identify open slots before creating a booking.

**Q: Can I set up webhooks for new bookings?**
Yes! Use `create_webhook` with your callback URL, events like 'invitee.created' and 'invitee.canceled', and the scope (your user or organization URI). Optionally provide a signing key for verification. You can audit existing webhooks with `list_webhooks`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calendly-alternative](https://vinkius.com/mcp/calendly-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calendly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calendly-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calendly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calendly-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
