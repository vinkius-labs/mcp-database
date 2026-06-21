# Fantastical MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fantastical)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage calendars via Fantastical — create events using natural language, handle scheduling openings and proposals, and monitor connected accounts directly from any AI agent.

## Description
Connect your **Fantastical** account to any AI agent and take full control of your unified calendar management and advanced scheduling through natural conversation.

### What you can do

- **Natural Language Event Orchestration** — Leverage Fantastical's elite parsing engine to create new events by commanding simple phrases like 'Lunch with Bob tomorrow at noon' natively
- **Unified Calendar Auditing** — Retrieve all scheduled events across Google, iCloud, Exchange, and Microsoft 365 in a single structural view within your chat
- **Scheduling Openings** — List and manage your shareable booking links where others can schedule time with you based on your real-time availability flawlessly
- **Meeting Proposals** — Suggest multiple time slots to attendees and track responses to finalize meeting times without manual back-and-forth
- **Reminder Management** — Create and audit task-like items with due dates that sync with Apple Reminders or Todoist natively alongside your calendar
- **Calendar Oversight** — Enumerate all connected providers and manage structural layouts identifying specific account colors and active statuses securely
- **Event Modification** — Update existing events by transmitting logical segments like titles, times, locations, or notes synchronously across all providers

### How it works

1. Subscribe to this server
2. Enter your Fantastical API Key (found in your Flexibits Account Hub under Integrations)
3. Start managing your calendar from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Busy Professionals** — manage multiple calendar providers and create events using natural language without leaving the chat interface
- **Executive Assistants** — coordinate meeting proposals and manage booking openings for teams using natural conversation
- **Developers** — test and debug calendar integrations and verify natural language parsing logic in real-time
- **Power Users** — audit unified schedules and manage reminders across different services through a single AI assistant


## Available Tools (10)
- **list_events**: Requires start and end dates.

List all calendar events in Fantastical within a date range
- **get_event**: Retrieve full details of a Fantastical event by ID
- **create_event**: Fantastical excels at parsing natural language — "Lunch with Bob tomorrow at noon".

Create a new event in Fantastical using natural language parsing
- **update_event**: Changes sync to the underlying calendar provider.

Update an existing Fantastical event
- **delete_event**: Delete a Fantastical event permanently
- **list_calendars**: Fantastical unifies calendars from multiple providers into one view.

List all calendars connected to Fantastical
- **list_openings**: List all Openings (scheduling pages) in Fantastical
- **get_opening**: Get details of a specific Fantastical Opening
- **list_proposals**: Returns proposal titles, suggested times, responses, and finalized slots.

List all Proposals in Fantastical
- **create_reminder**: They sync with Apple Reminders or Todoist depending on your setup.

Create a new reminder in Fantastical


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fantastical** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create event: 'Deep Work session tomorrow from 9am to 11am'"

**🤖 AI Agent:**
> Event created! I've added 'Deep Work session' to your calendar for tomorrow (March 31, 2026) from 9:00 AM to 11:00 AM. I used Fantastical's natural language engine to parse your request flawlessly.

---

**👤 You:**
> "List my events for this week"

**🤖 AI Agent:**
> Retrieving your schedule... You have 8 events this week across your connected calendars. Highlights include 'Product Review' on Wednesday and a 'Team Lunch' on Friday. Would you like the full list?

---

**👤 You:**
> "What are my active scheduling Openings?"

**🤖 AI Agent:**
> I found 2 active Openings: '15 Minute Coffee Chat' and '60 Minute Strategy Session'. I can provide the booking links for you to share.


## ❓ FAQ

**Q: Can my agent create events using natural language phrases like in the Fantastical app?**
Yes. Use the 'create_event' tool. Fantastical's engine is designed to parse phrases like 'Lunch with Bob at 1pm next Tuesday'. The agent will transmit the string and return the structured event data flawlessly.

**Q: How do I see my available scheduling links (Openings) via chat?**
Use the 'list_openings' tool. Your agent will retrieve all your active scheduling pages, providing the booking link URLs and duration settings so you can share them with others easily.

**Q: Can I suggest multiple meeting times to someone through the agent?**
Absolutely. Use the 'list_proposals' tool to monitor existing suggestions. Fantastical Proposals allow you to offer several slots to attendees, and your agent can help you track their responses and finalize the event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fantastical](https://vinkius.com/mcp/fantastical)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fantastical** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fantastical` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fantastical** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fantastical": {
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
