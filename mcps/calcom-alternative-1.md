# Cal.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calcom-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate scheduling via Cal.com — manage bookings, event types, and availability directly from any AI agent.

## Description
Connect your **Cal.com** account to any AI agent to streamline your scheduling workflows through natural conversation.

### What you can do

- **Booking Management** — Create, list, cancel, and reschedule bookings effortlessly without leaving your chat interface.
- **Event Types** — Define, list, and update meeting templates (event types) with specific durations and slugs.
- **Availability & Slots** — Query real-time available slots and busy times for specific users and event types.
- **Schedules & Teams** — Manage complex organizational schedules, team memberships, and out-of-office periods.
- **Webhooks & Credits** — Configure automation triggers and manage API usage credits for enterprise-level integrations.

### How it works

1. Subscribe to this server
2. Enter your Cal.com API Key
3. Start managing your calendar from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Support Teams** — instantly check availability and book meetings with leads without switching tabs.
- **Executives & Assistants** — reschedule or cancel appointments using simple natural language commands.
- **Developers** — integrate scheduling logic into automated workflows or custom AI agents.


## Available Tools
- **cancel_booking**: Cancel a booking
- **charge_credits**: Charge credits
- **create_booking**: Requires either eventTypeId OR (eventTypeSlug + username).

Create a new Cal.com booking
- **create_event_type**: Create a new event type
- **create_membership**: Create an organization membership
- **create_schedule**: Create a schedule
- **create_team**: Create a team
- **create_webhook**: Create a webhook
- **get_booking**: Get a specific booking by UID
- **get_busy_times**: Get busy times
- **get_credits**: Check available credits balance
- **get_me**: Get current user profile
- **get_slots**: Get available slots
- **list_bookings**: Get all bookings
- **list_event_types**: Get all event types
- **list_out_of_office**: Get all out-of-office (OOO) entries
- **list_schedules**: Get all schedules
- **reschedule_booking**: Reschedule a booking
- **update_event_type**: Update an event type
- **update_schedule**: Update a schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cal.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming bookings for this month."

**🤖 AI Agent:**
> I've retrieved your upcoming bookings. You have 3 meetings scheduled: 'Product Sync' on Oct 12, 'Client Onboarding' on Oct 15, and 'Team Retro' on Oct 18. Would you like details on any of these?

---

**👤 You:**
> "Check available slots for user 'johndoe' for the '15-min-chat' event next Monday."

**🤖 AI Agent:**
> Checking availability... For Monday, Oct 16, John Doe has available slots at 10:00 AM, 10:15 AM, 11:30 AM, and 2:00 PM (UTC). Should I book one of these for you?

---

**👤 You:**
> "Cancel my booking with UID 'bk_12345' because I have a conflict."

**🤖 AI Agent:**
> I have successfully cancelled booking 'bk_12345'. The reason provided was 'conflict'. A notification has been sent to the attendees.


## ❓ FAQ

**Q: Can I check when a user is available for a specific meeting type?**
Yes! Use the `get_slots` tool by providing the username, event slug, and a time range. The agent will return all available time slots for that period.

**Q: Is it possible to reschedule an existing booking through the AI?**
Absolutely. Use the `reschedule_booking` tool with the Booking UID and the new start time. You can also optionally provide a reason for the change.

**Q: Can I manage my organization's event templates?**
Yes, you can use `list_event_types` to see all templates, `create_event_type` to add new ones, and `update_event_type` to modify existing durations or titles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calcom-alternative-1](https://vinkius.com/mcp/calcom-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cal.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `calcom-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cal.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calcom-alternative-1": {
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
