# Truto Unified Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/truto-unified-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Empower your AI agent with a universal API to read, schedule, and sync events seamlessly across Google, Outlook, and other major calendar providers.

## Description
Deploy the ultimate scheduling machine by linking your AI agent to **Truto**. Instead of building fragmented code for individual calendar APIs, Truto provides a normalized schema that controls Google Calendar, Outlook, and countless others underneath. Command your agent to list daily events, find free timeslots accurately, or write absolute meetings directly to the chosen provider without swapping logic loops.

### What you can do

- **Unified Calendar Tracking** — Check all connected calendars regardless of provider natively and list their available events continuously
- **Meeting Generation** — Instruct your AI to generate or directly cancel/update specific events passing ISO-compliant timings directly to the root provider
- **Free/Busy Analysis** — Demand explicit gaps inside your schedule bypassing complex metadata just extracting readable unavailable/available blocks
- **Integration Audit** — Check the absolute status of all connected root provider connections (Integrations) to ensure nothing is decoupled abruptly
- **Event Forensics** — Interrogate and extract any granular metadata embedded inside an `event_id`, including conferencing details and attendee lists

### How it works

1. Anchor this multi-calendar instance to your local Vinkius conversational agent
2. Provide the Master Token from Truto combined specifically with your `Integrated Account ID` targeting a specific linked provider
3. Engage scheduling queries organically conversing with your assistant

### Who is this for?

- **Executive Assistants** — Book multi-provider meetings strictly through conversational commands checking calendar gaps dynamically
- **Sales Coordinators** — Force event creation securely across varied client infrastructures without logging into fragmented Google and Microsoft portals
- **Platform Architects** — Centralize routing logic manipulating the agent to alter calendar entries strictly using one unified schema rule


## Available Tools (10)
- **create_event**: Provide calendar_id, title, and start/end times in ISO format.

Create a new event in a calendar via Truto. The event is written through to the underlying provider (Google/Outlook) in real-time. Provide calendar ID, title, and ISO 8601 start/end times
- **delete_event**: This action is irreversible.

Delete an event via Truto. The event is removed from both Truto and the underlying provider in real-time
- **get_calendar**: Get details of a specific calendar via Truto by ID. Returns calendar name, provider, timezone, and metadata normalized to the Truto unified schema
- **get_event**: Get full details of a specific event via Truto. Returns title, description, start/end times, attendees, location, organizer, recurrence, and provider-specific metadata
- **get_free_busy**: Provide calendar_id and time range.

Get free/busy data for a calendar via Truto within a date range. Returns time blocks as free or busy in the unified Truto format
- **list_calendars**: List all calendars via Truto unified API. Truto provides a real-time, pass-through API that normalizes calendar data across Google Calendar, Outlook Calendar, and other providers into a consistent schema
- **list_connections**: List all integrated accounts (connections) in Truto. Shows connected calendar providers, auth status, and account metadata
- **list_events**: Provide the calendar_id.

List all events from a calendar via Truto. Returns events in a unified format regardless of the underlying provider. Shows titles, times, attendees, locations, and conferencing info
- **update_event**: Provide the event_id and a JSON updates object.

Update an existing event via Truto. Provide a JSON object with fields to change. Changes pass through to the real provider in real-time
- **validate_connection**: Validate a Truto integrated account connection. Checks credentials, permissions, and API accessibility. Returns validation status and any errors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Truto Unified Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all interconnected calendars belonging to this unified account."

**🤖 AI Agent:**
> Listing calendars for Integrated Account. Retrieved 2 major calendars:
1. 'Primary Operations' (ID: cal_91bx2) [Google Provider]
2. 'Global Holidays' (ID: cal_84zy1) [Google Provider].

---

**👤 You:**
> "Search my events and get the specific details for event ID evt_7xkP."

**🤖 AI Agent:**
> Details recovered. Meeting 'Q3 Alignment Sprint' goes from 2026-10-14T09:00Z to 2026-10-14T10:30Z. Video conferencing link appended natively. 4 attendees invited.


## ❓ FAQ

**Q: How and where do I collect my universal Truto API Token?**
Navigate accurately toward your primary Truto management dashboard portal. Search intentionally along your workspace or developer settings focusing clearly on the `API Keys` section. Dictate the explicit creation of a new bearer credential. Lock the generated long string into your clipboard and transport it perfectly to the waiting field array below.

**Q: What is the Truto Integrated Account ID and where is it?**
Because Truto is unified, one single environment connects entirely to many different client calendars (e.g., your Google, a client's Outlook). The `Integrated Account ID` designates explicitly WHICH underlying calendar provider the agent should orchestrate right now. You fetch this prefix ID commonly starting with `ia_` precisely from the Integrations tab listed inside your Truto dashboard.

**Q: Should I save the Truto API Token immediately?**
Yes. Once you click 'Create API Token' and it gets generated, you must copy it immediately. Truto will only show the API Token once. If you close the window without securely saving it, you will have to create a new one.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truto-unified-calendar](https://vinkius.com/mcp/truto-unified-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Truto Unified Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `truto-unified-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Truto Unified Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truto-unified-calendar": {
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
