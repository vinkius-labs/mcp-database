# Google Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Sync and orchestrate your agenda securely — scan, schedule, and manipulate Google Calendar events natively in chat.

## Description
Connect your **Google Calendar** network to any AI agent and optimize scheduling frictions cleanly. Let a dedicated AI calendar associate fetch meeting data, clear blocks, and establish appointments automatically.

### What you can do

- **Event Querying** — Look deep into the future and past, listing calendar entries, attendees, formats and link details (Google Meet/Zoom) with surgical precision
- **Booking Operations** — Act upon schedule overlaps by inserting new events autonomously right alongside notifications or existing tasks
- **Modification Hooks** — Automatically reschedule conflicting meetings or tweak descriptions and invite lines across dynamic workdays

### How it works

1. Subscribe to this server module
2. Introduce your OAuth framework credentials from Workspace/GCP
3. Direct the AI to manipulate your calendars

### Who is this for?

- **Project Managers** — instantly spot team sync anomalies or free slots to slot urgent crisis response meetings seamlessly
- **Founders & Execs** — delegate scheduling back-and-forths strictly through one coherent command block


## Available Tools
- **list_events**: List upcoming events from a specific calendar
- **list_event_instances**: List instances of a recurring event
- **move_event**: Move an event to a different calendar
- **check_free_busy**: Check availability for a specific time range
- **create_event**: Schedule a new event
- **delete_event**: Cancel/Delete an event
- **get_calendar_metadata**: Get metadata for a specific calendar
- **get_event**: Get details of a specific event
- **get_settings**: Get user calendar settings
- **list_acl**: List access control rules for a calendar
- **list_calendars**: List all calendars in the user account
- **patch_event**: Partially update an event (e.g., change just the status or attendees)
- **quick_add_event**: Create an event from a simple text string
- **search_events**: Search for events based on a text query
- **update_event**: Modify an existing event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my schedule for tomorrow and list the upcoming overlapping events."

**🤖 AI Agent:**
> Scanning the timeline for tomorrow... Between 14:00 and 15:00 UTC I detected two conflicting bookings: 'Q3 Board Review' and 'Design Synchronization Session'. Should I cancel the Design sync?

---

**👤 You:**
> "Book a 30-minute sync session with marketing@domain.com for next Tuesday at 10 AM."

**🤖 AI Agent:**
> Request finalized. Event 'Marketing Sync Session' successfully placed on the calendar for next Tuesday at 10:00 (Duration: 30m). An invite payload including Meet details was beamed to marketing@domain.com.

---

**👤 You:**
> "Modify the location of the event titled 'Team Dinner' to 'The Grand Plaza Downtown'."

**🤖 AI Agent:**
> Search pinpointed the item ('Team Dinner' // ID: c18ba29d). Location parameter swapped securely to 'The Grand Plaza Downtown'. Updates have been cascaded down successfully.


## ❓ FAQ

**Q: Can it automatically generate meet links when booking?**
Yes. When building the `create_event` request, the agent can structure event metadata that explicitly flags conferencing generation. You get a Google Meet URL seamlessly inside the payload.

**Q: How does the tool handle multiple calendars (e.g. personal and work)?**
It requires querying the primary or specified secondary calendar IDs. By default, it operates on 'primary'. You can command the agent to use `list_calendars` to pick and choose exactly which specific agenda it targets.

**Q: Will the AI delete historical meetings completely if I ask it?**
While specific `delete_event` tools track individual IDs, bulk deletions and catastrophic operations are architecturally suppressed for safety. Removing isolated tasks works strictly one-by-one by direct matching.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-calendar](https://vinkius.com/mcp/google-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-calendar": {
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
