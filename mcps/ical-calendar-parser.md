# iCal Calendar Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ical-calendar-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Parse exported .ics calendar files from Google Calendar, Apple Calendar, or Outlook local. Let your AI find free slots, count meetings, and manage your schedule.

## Description
Claude has no access to your local calendar. When you ask 'Do I have any free time tomorrow afternoon?', it simply cannot answer. But if you export your calendar as an `.ics` file (which every major calendar app supports), this MCP bridges the gap.

This engine uses a robust iCal parser to extract every event with its title, start/end times, location, and attendees into a clean JSON timeline. Sorted chronologically, the AI can instantly find conflicts, identify free slots, and generate weekly summaries of your schedule.

### The Superpowers

- **Universal Calendar Support:** Works with Google Calendar, Apple Calendar, Outlook, and any standard .ics file.
- **Chronological Sorting:** Events are automatically sorted by start date for timeline clarity.
- **Token-Safe:** Caps at 200 events to prevent context overflow.
- **100% Air-Gapped Privacy:** Your personal schedule stays on your machine.


## Available Tools (1)
- **parse_ical_calendar**: ics). Provide the absolute file path.

Parse a local .ics calendar export (Google Calendar, Apple Calendar, Outlook) into structured JSON events offline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iCal Calendar Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read my calendar export and tell me if I have any free time tomorrow afternoon."

**🤖 AI Agent:**
> Tomorrow afternoon you have a meeting from 2-3 PM and another from 4-5 PM. You're free from 3 PM to 4 PM.

---

**👤 You:**
> "How many meetings did I have this month? Group them by day of the week."

**🤖 AI Agent:**
> This month: Monday (8), Tuesday (6), Wednesday (5), Thursday (7), Friday (3). Total: 29 meetings.

---

**👤 You:**
> "Find all events that contain the word 'dentist' in my calendar."

**🤖 AI Agent:**
> Found 2 'dentist' events: June 15 at 10 AM and September 3 at 3 PM.


## ❓ FAQ

**Q: How do I export my Google Calendar?**
Go to calendar.google.com > Settings > Import & Export > Export. It downloads a .zip containing .ics files for each calendar.

**Q: Can it detect scheduling conflicts?**
Yes! Because events are sorted chronologically with start/end times, the AI can easily spot overlapping events and alert you.

**Q: Does it include recurring events?**
Yes, the parser expands recurring events according to the iCal RRULE specification, so each individual occurrence appears as its own entry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ical-calendar-parser](https://vinkius.com/mcp/ical-calendar-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iCal Calendar Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ical-calendar-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iCal Calendar Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ical-calendar-parser": {
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
