# iCal Calendar Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ical-calendar-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ical-calendar-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ical-calendar-parser-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **iCal Calendar Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ical-calendar-parser](https://vinkius.com/mcp/ical-calendar-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
